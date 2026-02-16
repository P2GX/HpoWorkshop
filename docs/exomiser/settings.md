# ⚙️ Exomiser Settings — Analysis Template

!!! abstract "What is this file?"
    This YAML file defines how Exomiser filters, scores, and prioritizes variants.  
    Think of it as the **analysis pipeline configuration** — every step from
    allele-frequency filtering to phenotype prioritization is controlled here.

---

## 🧠 Overview

The template below represents a typical **PASS_ONLY** analysis configuration.

Key concepts:

- **analysisMode** — which variants from the VCF are evaluated
- **inheritanceModes** — weights applied to genetic models
- **filters** — remove unlikely variants
- **prioritisers** — rank genes based on phenotype evidence

---

## 🧬 Analysis Mode

!!! info "PASS_ONLY"
    Only variants marked as `PASS` in the VCF are analysed.
    This avoids low-quality variant calls.

---

## 🧬 Inheritance Models

!!! tip "How weighting works"
    Larger numbers increase the importance of that inheritance model
    during scoring.

Examples:

- `AUTOSOMAL_RECESSIVE_COMP_HET` = strong weight (2.0)
- `AUTOSOMAL_DOMINANT` = lower weight (0.1)

---

## 🌍 Frequency Sources

These datasets help remove common population variants:

- UK10K
- gnomAD exomes (GNOMAD_E_*)
- gnomAD genomes (GNOMAD_G_*)

!!! note
    As of gnomAD v4, several legacy datasets (1000G, ESP, ExAC) are incorporated into gnomAD.

---

## 🔬 Pathogenicity Sources

The configuration uses:

- **REVEL**
- **MVP**

!!! warning "CADD / REMM"
    If you enable CADD or REMM, you must install the tabix files
    and update their paths in `application.properties`.

---

## 🧩 Analysis Steps Explained

The `steps` section defines the Exomiser pipeline.

Typical flow:

1. Variant filtering
2. Frequency filtering
3. Inheritance filtering
4. Phenotype prioritisation

!!! important
    `inheritanceFilter` and `omimPrioritiser` should run **after** all filters.

---

## 📄 Full YAML Configuration

??? example "Show Analysis Template (click to expand)"
    ```yaml
    ## Exomiser Analysis Template.
    ---
    analysisMode: PASS_ONLY
    inheritanceModes: {
      AUTOSOMAL_DOMINANT: 0.1,
      AUTOSOMAL_RECESSIVE_HOM_ALT:  0.1,
      AUTOSOMAL_RECESSIVE_COMP_HET: 2.0,
      X_DOMINANT: 0.1,
      X_RECESSIVE_HOM_ALT: 0.1,
      X_RECESSIVE_COMP_HET: 2.0,
      MITOCHONDRIAL: 0.2
    }

    frequencySources: [
      UK10K,
      GNOMAD_E_AFR,
      GNOMAD_E_AMR,
      GNOMAD_E_EAS,
      GNOMAD_E_NFE,
      GNOMAD_E_SAS,
      GNOMAD_G_AFR,
      GNOMAD_G_AMR,
      GNOMAD_G_EAS,
      GNOMAD_G_NFE,
      GNOMAD_G_SAS
    ]

    pathogenicitySources: [ REVEL, MVP, ALPHA_MISSENSE, SPLICE_AI ]

    steps: [
      failedVariantFilter: { },

      variantEffectFilter: {
        remove: [
          FIVE_PRIME_UTR_EXON_VARIANT,
          FIVE_PRIME_UTR_INTRON_VARIANT,
          THREE_PRIME_UTR_EXON_VARIANT,
          THREE_PRIME_UTR_INTRON_VARIANT,
          NON_CODING_TRANSCRIPT_EXON_VARIANT,
          UPSTREAM_GENE_VARIANT,
          INTERGENIC_VARIANT,
          REGULATORY_REGION_VARIANT,
          CODING_TRANSCRIPT_INTRON_VARIANT,
          NON_CODING_TRANSCRIPT_INTRON_VARIANT,
          DOWNSTREAM_GENE_VARIANT
        ]
      },

      frequencyFilter: {maxFrequency: 2.0},
      pathogenicityFilter: {keepNonPathogenic: true},
      inheritanceFilter: {},
      omimPrioritiser: {},
      hiPhivePrioritiser: {}
    ]
    ```
**Next Module:** [Running Exomiser with phenopacket](running.md){ .md-button .md-button--primary }