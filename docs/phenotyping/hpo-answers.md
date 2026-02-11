# Navigating the HPO Website: Hints and Solutions

This page provides the worked solutions for the introductory exercises. Use these to check your work or if you get stuck during the module.

---

## Exercise 1: Solution

To determine the number of genes associated with [Pulmonary insufficiency (HP:0010444)](https://hpo.jax.org/app/browse/term/HP:0010444){:target="_blank"}, the most reliable method is using the **Export associations** feature.

!!! success "Answer"
    At the time of this writing, there were **18 genes** associated with Pulmonary insufficiency. 

When you download the Excel file, your data should look similar to the screenshot below. Each row represents a unique gene-disease-phenotype relationship.

![Pulmonary insufficiency - associated genes](../img/pulmonary-insufficiency-genes.png){ width="800" }

---

## Exercise 2: Solution

The goal was to determine the "depth" of the term [Sutural cataract (HP:0010695)](https://hpo.jax.org/app/browse/term/HP:0010695){:target="_blank"} relative to the root term [Phenotypic abnormality (HP:0000118)](https://hpo.jax.org/app/browse/term/HP:0000118){:target="_blank"}.

While you can click through the parents on the HPO website, using the **Ontology Lookup Service (OLS)** provides a much clearer visual path.



![OLS view of sutural cataract](../img/sutural-cataract-ols.png){ width="800" }

!!! success "Answer"
    There are **7 links** (or "hops") between *Sutural cataract* and *Phenotypic abnormality*. Therefore, we say the **depth** of this term is **7**.

### Why Depth Matters
In computational phenotyping, the depth of a term is often used as a proxy for **Information Content (IC)**. Generally, the deeper a term is in the hierarchy, the more specific it is, and the more power it has to help reach a specific diagnosis.

---

**Next Module:** [Other HPO Browsers](browsers.md){ .md-button .md-button--primary }