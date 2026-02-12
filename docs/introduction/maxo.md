# Medical Action Ontology (MAxO)

 Medical Action Ontology (MAxO) is an ontology specifically designed to organize medical procedures, therapies, and interventions. MAxO encompasses 1903 terms that can be used to annotate phenotypic features associated with specific diseases (using HPO and Mondo). For instance, the term [brain CT (MAXO:0010316)](https://www.ebi.ac.uk/ols4/ontologies/maxo/classes/http%253A%252F%252Fpurl.obolibrary.org%252Fobo%252FMAXO_0010316){:target="_blank"} can be linked to phenotypic features that can be ascertained using this method, such as ][Agenesis of corpus callosum (HP:0001274)](https://hpo.jax.org/browse/term/HP:0001274){:target="_blank"}. Presently, there are over 16,000 MAxO diagnostic annotations that target HPO terms. 
 
 
!!! abstract "MAxO diagnostic annotations"

    ![Annotation model](../img/maxoNetwork.png){ align=center width="100%" }

    Example disease annotations for [Familial cold autoinflammatory syndrome 2](https://hpo.jax.org/browse/disease/OMIM:611762){:target="_blank"}.
 
 
The MAxO project also includes annotations about disease-specific treatments for RDs. Each annotation identifies a medical action and its relationship to a disease or disease manifestation. The MAxO term’s relation to the disease or disease manifestation is specified by one of five relations. Some medical actions target the disease itself; for instance, fava bean intake avoidance (MAXO:0010051) can—in principle—prevent all clinical manifestations of G6PD deficiency (MONDO:0005775). In other cases, treatment is specific to a subset of disease manifestations. For instance, removal of the lens (MAXO:0001220) can be used to treat lens dislocation in Marfan syndrome (MONDO:0007947), but this measure does not treat other manifestations of Marfan syndrome such as aortic root dilatation. Fig. 4 shows an overview of the annotation model.

!!! abstract "MAxO therapeutic annotations"

    ![Annotation model](../img/maxoModel.png){ align=center width="40%" }

    Here, the indicated medical action is a specific nutrition intake avoidance, which if realized, means that hemolytic anemia will be prevented.


<div class="grid cards" markdown>

-   :material-book-open-page-variant:{ .lg .middle } __MAxO__

    ---

    *The Medical Action Ontology: A tool for annotating and analyzing treatments and clinical management of human disease.*

    [:material-open-in-new: PMID: 18950739](https://pubmed.ncbi.nlm.nih.gov/37963467/){:target="_blank" .md-button }

</div>


**Next Module:** [Clinical phenotyping](../phenotyping/hpobrowser.md){ .md-button .md-button--primary }