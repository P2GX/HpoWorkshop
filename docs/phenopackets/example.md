# Phenopacket Example — Netherton Syndrome

!!! abstract "Overview"
    This page presents a **Phenopacket v2.0.2** describing a male infant with  
    **OMIM:256500 — Netherton syndrome**, caused by a pathogenic variant in **SPINK5**.  





??? example "Show raw Phenopacket JSON"
    ```json
    {
        "id": "PMID_11952552_patient",
        "subject": {
            "id": "patient",
            "timeAtLastEncounter": {
            "age": {
                "iso8601duration": "P4M"
            }
            },
            "vitalStatus": {
            "status": "DECEASED"
            },
            "sex": "MALE"
        },
        "phenotypicFeatures": [
            {
            "type": {
                "id": "HP:0012472",
                "label": "Eclabion"
            },
            "excluded": true
            },
            {
            "type": {
                "id": "HP:0000656",
                "label": "Ectropion"
            },
            "excluded": true
            },
            {
            "type": {
                "id": "HP:0001019",
                "label": "Erythroderma"
            },
            "onset": {
                "ontologyClass": {
                "id": "HP:0003577",
                "label": "Congenital onset"
                }
            }
            },
            {
            "type": {
                "id": "HP:0025092",
                "label": "Epidermal acanthosis"
            }
            },
            {
            "type": {
                "id": "HP:0040190",
                "label": "White scaling skin"
            },
            "onset": {
                "ontologyClass": {
                "id": "HP:0003577",
                "label": "Congenital onset"
                }
            }
            },
            {
            "type": {
                "id": "HP:0010783",
                "label": "Erythema"
            }
            },
            {
            "type": {
                "id": "HP:0003777",
                "label": "Pili torti"
            }
            }
        ],
        "interpretations": [
            {
            "id": "7FevHw7ZYG6vwkStfPR4LfVa",
            "progressStatus": "SOLVED",
            "diagnosis": {
                "disease": {
                "id": "OMIM:256500",
                "label": "Netherton syndrome"
                },
                "genomicInterpretations": [
                {
                    "subjectOrBiosampleId": "patient",
                    "interpretationStatus": "CAUSATIVE",
                    "variantInterpretation": {
                    "acmgPathogenicityClassification": "PATHOGENIC",
                    "therapeuticActionability": "UNKNOWN_ACTIONABILITY",
                    "variationDescriptor": {
                        "id": "c153del_SPINK5_NM_006846v4",
                        "geneContext": {
                        "valueId": "HGNC:15464",
                        "symbol": "SPINK5"
                        },
                        "expressions": [
                        {
                            "syntax": "hgvs.c",
                            "value": "NM_006846.4:c.153del"
                        },
                        {
                            "syntax": "hgvs.g",
                            "value": "NC_000005.10:g.148070394del"
                        },
                        {
                            "syntax": "hgvs.p",
                            "value": "NP_006837.2:p.(Gln52LysfsTer6)"
                        }
                        ],
                        "vcfRecord": {
                        "genomeAssembly": "hg38",
                        "chrom": "chr5",
                        "pos": 148070388,
                        "ref": "AT",
                        "alt": "A"
                        },
                        "moleculeContext": "genomic",
                        "allelicState": {
                        "id": "GENO:0000136",
                        "label": "homozygous"
                        }
                    }
                    }
                }
                ]
            }
            }
        ],
        "diseases": [
            {
            "term": {
                "id": "OMIM:256500",
                "label": "Netherton syndrome"
            },
            "onset": {
                "ontologyClass": {
                "id": "HP:0003577",
                "label": "Congenital onset"
                }
            }
            }
        ],
        "metaData": {
            "created": "2025-12-31T15:52:33.505831Z",
            "createdBy": "0000-0002-0736-9199",
            "resources": [
            {
                "id": "hp",
                "name": "human phenotype ontology",
                "url": "http://purl.obolibrary.org/obo/hp.owl",
                "version": "2025-11-24",
                "namespacePrefix": "HP",
                "iriPrefix": "http://purl.obolibrary.org/obo/HP_"
            },
            {
                "id": "geno",
                "name": "Genotype Ontology",
                "url": "http://purl.obolibrary.org/obo/geno.owl",
                "version": "2025-07-25",
                "namespacePrefix": "GENO",
                "iriPrefix": "http://purl.obolibrary.org/obo/GENO_"
            },
            {
                "id": "so",
                "name": "Sequence types and features ontology",
                "url": "http://purl.obolibrary.org/obo/so.owl",
                "version": "2024-11-18",
                "namespacePrefix": "SO",
                "iriPrefix": "http://purl.obolibrary.org/obo/SO_"
            },
            {
                "id": "omim",
                "name": "An Online Catalog of Human Genes and Genetic Disorders",
                "url": "https://www.omim.org",
                "version": "06/01/25",
                "namespacePrefix": "OMIM",
                "iriPrefix": "https://www.omim.org/entry/"
            },
            {
                "id": "hgnc",
                "name": "HUGO Gene Nomenclature Committee",
                "url": "https://www.genenames.org",
                "version": "06/01/25",
                "namespacePrefix": "HGNC",
                "iriPrefix": "https://www.genenames.org/data/gene-symbol-report/#!/hgnc_id/"
            }
            ],
            "phenopacketSchemaVersion": "2.0.2",
            "externalReferences": [
            {
                "id": "PMID:11952552",
                "description": "Genetic analysis of a severe case of Netherton syndrome and application for prenatal testing"
            }
            ]
        }
    }
    ```

---

## 🧬 Patient Summary

| Field | Value |
|---|---|
| **Patient ID** | `PMID_11952552_patient` |
| **Sex** | Male |
| **Age at last encounter** | 4 months |
| **Vital status** | :material-close-circle: Deceased |
| **Primary diagnosis** | OMIM:256500 — Netherton syndrome |
| **Gene** | `SPINK5` |
| **Variant** | `NM_006846.4:c.153del` |

!!! info "Clinical context"
    Netherton syndrome is an autosomal recessive disorder characterized by congenital erythroderma,
    ichthyosis, and hair shaft abnormalities such as *pili torti*.

---

## 🧾 Phenotypic Features

=== "✅ Observed"

    | HPO ID | Label | Onset |
    |---|---|---|
    | `HP:0001019` | **Erythroderma** | Congenital |
    | `HP:0025092` | Epidermal acanthosis | — |
    | `HP:0040190` | White scaling skin | Congenital |
    | `HP:0010783` | Erythema | — |
    | `HP:0003777` | Pili torti | — |

    !!! tip
        Observed features contribute positively to phenotype-driven diagnostics.

=== "❌ Explicitly Excluded"

    | HPO ID | Label |
    |---|---|
    | `HP:0012472` | Eclabion |
    | `HP:0000656` | Ectropion |

    !!! warning "Why exclusions matter"
        Explicitly excluded phenotypes help narrow differential diagnoses
        and improve computational ranking algorithms.

---

## 🧬 Genetic Interpretation

!!! success "Causative Variant Identified"
    **Gene:** HGNC:15464 — `SPINK5`  
    **Allelic state:** Homozygous  
    **ACMG classification:** Pathogenic  
    **Interpretation status:** Causative

### Variant Expressions

| Syntax | Value |
|---|---|
| hgvs.c | `NM_006846.4:c.153del` |
| hgvs.g | `NC_000005.10:g.148070394del` |
| hgvs.p | `NP_006837.2:p.(Gln52LysfsTer6)` |

### VCF Representation

| Assembly | Chrom | Pos | Ref | Alt |
|---|---|---|---|---|
| hg38 | chr5 | 148070388 | AT | A |

!!! note "Interpretation"
    This frameshift deletion leads to premature truncation of the SPINK5 protein,
    consistent with loss-of-function variants reported in Netherton syndrome.

---

## 🧾 Disease

| Field | Value |
|---|---|
| Disease | `OMIM:256500` — Netherton syndrome |
| Onset | Congenital onset |

---

## 📚 Metadata

| Field | Value |
|---|---|
| Schema Version | 2.0.2 |
| Created | 2025-12-31 |
| External Reference | PMID:11952552 |

### Ontology Resources

- Human Phenotype Ontology (HP)
- Genotype Ontology (GENO)
- Sequence Ontology (SO)
- OMIM
- HGNC

---


**Next Module:** [Exomiser](../exomiser/index.md){ .md-button .md-button--primary }