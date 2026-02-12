# What is an ontology?

A goal of precision medicine1 is to stratify patients in order to improve diagnosis and medical treatment. Translational investigators are bringing to bear ever greater amounts of heterogeneous clinical data and scientific information to create classification strategies that enable the matching of intervention to underlying mechanisms of disease in subgroups of patients. Ontologies are systematic representations of knowledge that can be used to inte-grate and analyze large amounts of heterogeneous data, allowing precise classification of a patient.

## Ontology vs Terminology

A terminology is the set of all terms (concepts) of a domain.

Ontologies differ from terminologies in that ontologies define relationships between concepts in a way that allows computational logical reasoning, enabling the drawing of conclusions from related assertions. For example, if an ontology classifies “virus” as an infectious agent and classifies “infectious meningitis” as a type of meningitis due to an infectious agent, then it would conclude that “viral meningitis” is a subclass of “infectious meningitis.” Aristotle developed conceptual taxonomies that are in some ways similar to modern bio-ontologies.13 More recently, scientists have used the word “ontology” to denote a computational representation describing specific domains of knowledge. An ontology consists of a set of concepts (terms) and their synonyms, as well as description-logic definitions that specify the formal relationships between the concepts.



!!! abstract "Ontology-Driven Representation of Fanconi Anemia and Acquired Aplastic Anemia"
    ![Phenoboard](../img/nejm-fanconi.png){ align=center }
    
    Fanconi anemia and acquired aplastic anemia share several phenotypic features but have very different causal mechanisms. Computable relationships can be represented among diseases, phenotypic features, genes, and environmental exposures by interlinking terms (concepts) from sources including the Orphanet Rare Disease ontology (ORDO) (pink denotes diseases),14 the Human Phenotype Ontology (HPO)15 for phenotypic features (orange), the Chemical Entities of Biological Interest ontology for the chemical compounds (green denotes factors such as chemical exposures that can influence severity or trigger development of disease),16 and the Ontology for Biomedical Investigations for the comet assay (single-cell gel-electrophoresis assay) of DNA breakage (aqua),17 as well as the Gene Ontology (lavender denotes a biologic pathway)18 and the Reactome for molecular pathways (blue denotes disease genes and mode of inheritance).19 Ontologies can be used to support the integrative analysis of these data sources for precision stratification and treatment and to clarify underlying mechanisms, as suggested by the dashed lines. The labeled arrows between concepts represent description-logic definitions that specify the formal relationships between the concepts. FA-A denotes Fanconi anemia, complementation group A; FA-B, complementation group B; and so on. In the diagram of the Fanconi anemia pathway, the blue circles represent the proteins encoded by the Fanconi genes (e.g., A is the protein encoded by FANCA), and the grayish-blue ovals represent other interacting proteins; P denotes phosphorylation, and ub ubiquitination.


**Next Module:** [HPO Annotations](annotation.md){ .md-button .md-button--primary }