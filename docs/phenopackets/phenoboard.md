# :material-view-dashboard-outline: Phenoboard

[GA4GH Phenoboard](https://github.com/P2GX/phenoboard) is a desktop application (Tauri-based) designed to help curate cohorts of individuals with rare genetic disease using the **GA4GH Phenopacket Schema**.

In this workshop, we will use it to create a phenopacket that we will use to run the **Exomiser** in the final module.

---

!!! abstract "GA4GH Phenoboard"
    ![Phenoboard](../img/phenoboard-screenshot.png){ align=center width="85%"}
    
     **Phenoboard** is a desktop application for curatiing clinical cases using HPO and the
     GA4GH Phenopacket.

---

## :material-download: Installation

See the [Phenoboard documentation](https://p2gx.github.io/phenoboard/) for insformation about installing and setting up phenoboard on your laptop.

---

## :material-file-document-outline: Case report

The following clinical description was taken from [PMID:16614535](https://pubmed.ncbi.nlm.nih.gov/16614535/) and can be used for text mining in phenoboard.

!!! quote "Pfeiffer syndrome case report"

    A girl was delivered by spontaneous normal vaginal delivery at 38 weeks gestation after an unremarkable pregnancy. She was 3.5 kg in weight (25-50 percentile), the head circumference was 33 cm (25-50 percentile), and the height at birth was 52 cm (25-50 percentile).

    Upon birth, the infant demonstrated bilaterally fused coronal sutures, mild proptosis, and maxillary hypoplasia. The soft tissues of her 2nd, 3rd and 4th fingers were fused bilaterally to the proximal portion of distal phalanx and her bilateral thumbs were broad and deviated radially. Syndactyly of the feet involving all 5 toes was observed. The infant demonstrated evidence of respiratory distress with choanal hypoplasia. There was no deformity or motion limitation of bilateral elbows or shoulder joints.

    Head photography of 2 week-old girl shows a brachicephalic head as a result of bilateral coronal synostosis, and regressed small mid-face with mild proptosis. Hand photography shows bilateral syndactyly of 2nd, 3rd, and 4th fingers with broad and radially-deviated thumbs.

---

## :material-play-circle-outline: Running Phenoboard

We will demonstrate how to use phenoboard for this case during the workshop. We will require the following data:


| Field | Value |
|---|---|
| Disease identifier | **OMIM:101600** |
| Disease name | Pfeiffer syndrome |
| Gene symbol | FGFR2 |
| Transcript | NM_000141.5 |
| HGNC id | HGNC:3689 |

---

### :material-dna: Variant to enter

During the exercise, enter the following pathogenic variant:

- **Gene:** FGFR2  
- **cDNA:** c.1988G>A  
- **Protein:** p.Gly663Glu  
- ClinVar record: https://www.ncbi.nlm.nih.gov/clinvar/variation/2735492/

This corresponds to a missense variant associated with Pfeiffer syndrome.

**Next Module:** [Example phenopacket](example.md){ .md-button .md-button--primary }