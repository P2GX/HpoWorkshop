# 🧬 Exomiser

!!! abstract "What is Exomiser?"
    **Exomiser** is a phenotype-driven variant and gene prioritization tool designed for  
    next-generation sequencing (NGS) analysis in Mendelian disease.  
    It integrates **genetic variant data** with **Human Phenotype Ontology (HPO)** annotations  
    to rank candidate disease genes for diagnosis or novel gene discovery.

---

## 📖 Key References

- Robinson PN *et al.* (2014)  
  *Improved exome prioritization of disease genes through cross-species phenotype comparison.*  
  **Genome Research** 24(2):340-348.  
  [PMID:24162188](https://pubmed.ncbi.nlm.nih.gov/24162188/)

- Smedley D (2015)  
  *Next-generation diagnostics and disease-gene discovery with the Exomiser.*  
  **Nature Protocols** 10(12):2004-2015.  
  [PMID:26562621](https://pubmed.ncbi.nlm.nih.gov/26562621/)

---

## 🧪 Background

Exomiser was among the first phenotype-aware prioritization tools and was released in 2014  
as a freely available Java application.

It requires two primary inputs:

1. **Genomic data**
   - A VCF file containing variants from a rare-disease patient  
   - Optionally, a multi-sample VCF and a pedigree (`PED`) file for family analyses

2. **Phenotypic data**
   - A list of **HPO terms** describing the patient’s clinical features

The algorithm combines variant pathogenicity predictions with phenotype similarity scoring
across human and model-organism data.

---

## 🚀 Online Demo

A demo version of Exomiser is available here:

👉 https://exomiser.monarchinitiative.org/exomiser/

---

## 🧬 Hands-On Exercise

!!! tip "Goal"
    Learn how phenotype-driven prioritization improves variant interpretation.

Download the provided example dataset containing:

- An exome from a healthy individual
- A **causative FGFR2 variant** associated with autosomal dominant **Pfeiffer syndrome**

### Step 1 — Add Phenotypes

Add HPO terms describing Pfeiffer syndrome, similar to the workflow used in Phenomizer.

You may consult the HPO disease page:

👉 https://hpo.jax.org/app/browse/disease/OMIM:101600

### Step 2 — Run Exomiser

You can:

- Run Exomiser using **default settings**, or
- Adjust parameters (see the publications above for detailed explanations).

---

## 🧾 Exercise 1

!!! question "Explore the results"
    Examine the Exomiser output and answer the following:

- What are the **top five candidate genes**?
- What phenotypic evidence supports their ranking?
- What genetic evidence argues for or against each candidate?

Consider:

- Variant pathogenicity scores
- Phenotype similarity scores
- Mode of inheritance
- Gene–disease associations

