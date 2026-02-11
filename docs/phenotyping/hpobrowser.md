# Navigating the HPO Website

This page contains a series of exercises that illustrate how to find information on the [Human Phenotype Ontology (HPO)](https://hpo.jax.org/app/){:target="_blank"} website.

## The Basics

Go to the [HPO Start Page](https://hpo.jax.org/app/){:target="_blank"}. You will find a search box that offers autocomplete functionality.

![Main search field](../img/hpo-main-search.png){width="700"}

You can search for HPO terms, diseases, and genes. Let's start by searching for **Pulmonary insufficiency**. Enter it in the search window and click on the link. You should arrive at the page for [Pulmonary insufficiency (HP:0010444)](https://hpo.jax.org/app/browse/term/HP:0010444){:target="_blank"}.

The page offers several components. The core information about the term is shown in the header box.

![Pulmonary insufficiency](../img/pulmonary-insufficiency.png){width="800"}

### Key Term Elements
* **Primary Identifier:** `HP:0010444`
* **Preferred Label:** Pulmonary insufficiency
* **Definition:** A formal medical description of the term.
* **Synonyms:** Alternative names used to help find terms and support text mining.

Most HPO terms are used to annotate one or more diseases. In this case, Pulmonary insufficiency is used to annotate a number of diseases shown in the **Disease Associations** tab.

![Pulmonary insufficiency diseases](../img/pulmonary-insufficiency-diseases.png){width="800"}

The **Gene Associations** tab shows the genes that are associated with these diseases.

---

!!! example "Exercise 1: Gene Associations"
    **Goal:** Determine how many genes are associated with pulmonary insufficiency in the HPO data resource. 
    
    *Note: A gene is "associated" if a pathogenic variant in that gene causes a Mendelian disease that manifests as pulmonary insufficiency.*

    **How to answer:**
    1. Check the **Genes** tab on the term page for a live list.
    2. Click the **Export associations** button to download an Excel file containing the gene list.
    
    **Action:** Download the Excel file and count the unique gene entries.

---

## The HPO Hierarchy

Each term in the HPO describes a phenotypic abnormality. Terms are related to "parent" terms by **"is a"** relationships. The structure of the HPO allows a term to have multiple parent terms, enabling different aspects of phenotypic abnormalities to be explored. 

### The True-Path Rule
The "true-path rule" applies here: if an individual has a specific condition, they are also considered to have all the broader parent conditions. 

For example, if an individual has [Sutural cataract](https://hpo.jax.org/app/browse/term/HP:0010695){:target="_blank"}, they also technically have:
1. The parent: [Zonular cataract](https://hpo.jax.org/app/browse/term/HP:0010920){:target="_blank"}
2. The grand-parent: [Cataract](https://hpo.jax.org/app/browse/term/HP:0000518){:target="_blank"}



The HPO is constructed to capture medical knowledge in this hierarchical way. Therefore, navigating this "tree" is a vital skill.

---

!!! example "Exercise 2: Calculating Term Depth"
    **Goal:** Determine the number of links (hops) from [Sutural cataract](https://hpo.jax.org/app/browse/term/HP:0010695){:target="_blank"} to the root of the phenotypic abnormality section: [Phenotypic abnormality (HP:0000118)](https://hpo.jax.org/app/browse/term/HP:0000118){:target="_blank"}.

    **Instructions:**
    1. Note that there is **one link** between *Sutural cataract* and *Zonular cataract*.
    2. Navigate from a term to its parent using the hierarchy box on the HPO website.
    3. Count the number of "clicks" it takes to reach the top-level term *Phenotypic abnormality*.
    
    **Alternative Method:**
    Use the [EBI Ontology Lookup Service (OLS)](https://www.ebi.ac.uk/ols/ontologies/hp/terms?iri=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FHP_0010695){:target="_blank"}. This browser shows the entire path from the selected term to the root in one view, allowing you to count the links directly.

![Hierarchy of term sutural cataract](../img/sutural-cataract-hierarchy.png){width="800"}

---

## Wrap-up

In this module, you have learned to:
* Recognize basic elements of an HPO term (ID, Label, Definition, Synonyms).
* Search for HPO terms using the official web portal.
* Identify diseases and genes associated with a specific phenotype.
* Navigate the hierarchy to determine a term's **depth**.

??? tip "Stuck on an exercise?"
    If you had trouble with any of these tasks, you can check the [Exercise Answers](./hpo-answers.md) page for a full walkthrough.