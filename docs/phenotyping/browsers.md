# HPO Browser Comparison

While the official HPO website is the primary resource for clinicians, researchers often use secondary "Ontology Browsers" to explore complex relationships or download data in different formats.

## 1. HPO Browser (Official)
**Best for:** Clinical information and disease-gene associations.

* **URL:** [hpo.jax.org](https://hpo.jax.org/app/){:target="_blank"}
* **Unique Feature:** Provides clinical synonyms, "Layperson" terms, and direct links to OMIM/Orphanet diseases.
* **Visuals:** Shows a "local" hierarchy (immediate parents and children only).



## 2. EBI Ontology Lookup Service (OLS)
**Best for:** Visualizing the full hierarchy path.

* **URL:** [ebi.ac.uk/ols](https://www.ebi.ac.uk/ols/ontologies/hp){:target="_blank"}
* **Unique Feature:** The **Tree View**. Unlike the official site, OLS shows the entire lineage from the root (Phenotypic Abnormality) down to your specific term in one single tree.
* **Great for:** Calculating "Term Depth" or seeing how a term inherits properties from multiple parents.



## 3. Ontobee
**Best for:** Deep technical metadata and Linked Data (RDF/OWL).

* **URL:** [ontobee.org](http://www.ontobee.org/ontology/HP){:target="_blank"}
* **Unique Feature:** Focuses on the logic and URIs. It is the "source of truth" for how the ontology is coded in the Web Ontology Language (OWL).
* **Great for:** Bioinformaticians who need the exact permanent URI or SPARQL endpoints.

---

## Comparison Summary

| Feature | HPO Browser | EBI OLS | Ontobee |
| :--- | :--- | :--- | :--- |
| **Primary Audience** | Clinicians / Geneticists | Data Scientists | Ontologists |
| **Hierarchy View** | Local (Immediate) | Full Tree & Graph | List-based |
| **Disease Data** | Yes (Extensive) | Limited | None |
| **Term Depth** | Hard to count | Very easy to count | Difficult |

---

!!! info "Exercise: Browser Scavenger Hunt"
    Search for **"Hypotonia" (HP:0001252)** in all three browsers to see the difference in perspective:
    
    1. **HPO:** Find one "Layperson" synonym for Hypotonia.
    2. **OLS:** Use the **Tree View** to see how many "hops" it is from the root.
    3. **Ontobee:** Locate the **URI** (e.g., `http://purl.obolibrary.org/obo/HP_0001252`).

---

## Quick Launch Links
Use these links to jump to the entry for **Sutural Cataract (HP:0010695)** in each tool:

* [View in HPO Browser](https://hpo.jax.org/app/browse/term/HP:0010695){:target="_blank"}
* [View in EBI OLS](https://www.ebi.ac.uk/ols/ontologies/hp/terms?iri=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FHP_0010695){:target="_blank"}
* [View in Ontobee](http://www.ontobee.org/ontology/HP?iri=http://purl.obolibrary.org/obo/HP_0010695){:target="_blank"}