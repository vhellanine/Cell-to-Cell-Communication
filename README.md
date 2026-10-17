# Cell-to-Cell Communication: NK Cell to Macrophage

## Student Information
- **Student Name:** Junavhel Jane B. Olaguir
- **Course/Section:** BS Biology – [Insert Section]
- **Organism:** *Homo sapiens*
- **Chosen Sender Cell:** Natural Killer (NK) Cell
- **Receiver Cell:** Macrophage

---

## 1. Biological Question

How can a natural killer (NK) cell communicate with a macrophage through interferon-gamma (IFN-γ), and what intracellular signaling events may occur after the signal is received?

This activity investigates a proposed cell-to-cell communication pathway using biological databases. The investigation focuses on the candidate signaling molecule, its receptor, the associated protein network, and the possible cellular response of the receiver cell.

## 2. Chosen Sender Cell and Biological Context

The selected sender cell is the natural killer (NK) cell, an immune cell involved in the innate immune response. NK cells can recognize and eliminate certain virus-infected and tumor cells. They can also release cytokines that influence the activities of other immune cells.

The biological context selected for this activity is immune activation and communication between NK cells and macrophages.

The proposed communication is **paracrine signaling**, in which a secreted signaling molecule acts on another cell. A macrophage was selected as the receiver cell because it can respond to IFN-γ during immune activation.

## 3. Candidate Ligand and Evidence for Sender-Cell Expression

The candidate signaling molecule is **interferon-gamma (IFN-γ)**, encoded by the *IFNG* gene. IFN-γ is a cytokine involved in immune regulation and the activation of cellular defense mechanisms.

The Human Protein Atlas was used to examine *IFNG* expression in NK cells. The screenshot of the HPA single-cell expression page showed the following values:

| Dataset | Reported expression |
|---|---:|
| HPA | 0.9 nTPM |
| Monaco | 57.4 nTPM |
| Schmiedel | 134.6 TPM |

The HPA dataset displayed six NK-cell samples, with expression values ranging from 0.0 to 3.3 nTPM. The results varied across datasets, showing that the reported expression levels depend on the dataset examined.

These findings support investigating IFN-γ as a candidate signal produced by NK cells. However, RNA expression alone does not prove that the cytokine was secreted under a particular physiological condition.

**Evidence file:** `figures/01_sender_cell_evidence.png`

## 4. Receptor and Receiver Cell

The proposed receiver cell is a macrophage, and the candidate receptor is the interferon-gamma receptor complex, consisting of IFNGR1 and IFNGR2.

The OmniPath search for *IFNG* displayed an interaction from IFNG to IFNGR1. The results also showed an association involving IFNG and STAT1. These findings helped identify relevant components for further investigation of the proposed signaling mechanism.

IFNGR1 and IFNGR2 are the receptor subunits involved in IFN-γ signaling. Following receptor activation, the JAK–STAT pathway can transmit the signal inside the receiver cell.

The proposed signaling sequence is:

**NK cell → IFN-γ → IFNGR1/IFNGR2 → JAK1/JAK2 → STAT1 → Changes in gene expression**

The macrophage was selected as the receiver because macrophages can respond to IFN-γ. Nevertheless, the database results must be interpreted alongside evidence of receptor expression and the biological context of the selected cells.

**Evidence files:**
- `figures/02_omnipath_IFNG.png`
- `figures/02a_omnipath_IFNGR1.png`
- `figures/02b_omnipath_IFNGR2.png`

## 5. OmniPath Findings

OmniPath was used to examine signaling relationships involving IFNG and its associated proteins.

The search results displayed:
- An interaction from IFNG to IFNGR1.
- An association involving IFNG and STAT1.
- Additional signaling relationships involving proteins such as TBX21 and RELB.

The IFNG–IFNGR1 result was particularly relevant because it supported investigating IFNGR1 as a receptor component for the proposed signal. STAT1 was also included in the investigation because it is an important downstream transcription factor in IFN-γ signaling.

The OmniPath results provide evidence of annotated signaling relationships, but they do not independently demonstrate that the complete pathway occurs between the selected NK cell and macrophage.

## 6. STRING Network Analysis

STRING was used to examine functional associations among proteins related to the proposed signaling pathway.

The generated network contained the following statistics:

| Network statistic | Result |
|---|---:|
| Number of nodes | 11 |
| Number of edges | 55 |
| Expected number of edges | 16 |
| PPI enrichment p-value | 8.76 × 10⁻¹⁵ |

The network included proteins such as IFNGR1, IFNGR2, JAK1, JAK2, STAT1, STAT3, SOCS1, and TYK2.

### Relevant Proteins

- **IFNGR1:** A subunit of the IFN-γ receptor complex.
- **IFNGR2:** The second subunit of the IFN-γ receptor complex.
- **JAK1:** A receptor-associated kinase involved in intracellular signal transmission.
- **JAK2:** Another kinase involved in IFN-γ receptor signaling.
- **STAT1:** A transcription factor that regulates gene expression following activation.

### Enriched Biological Processes

The STRING functional-enrichment results included the following terms:

| Biological process | False discovery rate |
|---|---:|
| Type II interferon-mediated signaling pathway | 1.53 × 10⁻¹⁷ |
| Cell surface receptor signaling pathway via JAK-STAT | 6.89 × 10⁻¹⁸ |
| Interferon-mediated signaling pathway | 8.76 × 10⁻¹⁸ |
| Cellular response to virus | 1.40 × 10⁻¹⁴ |
| Type III interferon-mediated signaling pathway | 5.27 × 10⁻¹² |

The cell surface receptor signaling pathway via JAK-STAT was selected as the most relevant enriched process for the proposed model. The type II interferon-mediated signaling pathway was also relevant because IFN-γ belongs to the type II interferon family.

The PPI enrichment result indicates that the network contains more protein associations than expected for a random set of proteins of comparable size. However, STRING associations do not necessarily represent direct physical interactions or establish the direction of signaling.

**Evidence files:**
- `figures/03_string_network.png`
- `figures/03_string_enrichment.png`

## 7. IntAct Molecular Interaction Validation

IntAct was used to investigate an interaction between IFNG and IFNGR1.

The selected interaction record provided the following information:

| Item | Result |
|---|---|
| Interacting molecules | IFNG and IFNGR1 |
| IntAct accession | EBI-64053318 |
| Interaction type | Physical association |
| Detection method | Solid phase assay |
| Host organism | In vitro |
| Publication PMID | 32822567 |
| Positive interaction | Yes |

The associated publication is *A Human IgSF Cell-Surface Interactome Reveals a Complex Network of Protein-Protein Interactions*, published in 2020.

The IntAct record reports a positive physical association between IFNG and IFNGR1 under the listed experimental conditions. This provides relevant interaction evidence for the proposed ligand–receptor relationship.

However, the assay context must be considered when interpreting the result. The record alone does not establish that the interaction occurs under every physiological condition or prove the complete NK cell-to-macrophage signaling pathway.

**Evidence file:** `figures/04_intact_interaction_details.png`

## 8. Final Cell-to-Cell Communication Model

The proposed model illustrates how an NK cell may communicate with a macrophage through IFN-γ.

The sequence begins with the release of IFN-γ from the NK cell into the extracellular space. The cytokine can bind to the IFNGR1/IFNGR2 receptor complex on the macrophage. Receptor activation can then involve JAK1 and JAK2, followed by STAT1 activation and changes in gene expression.

These events may contribute to macrophage activation, including changes in antimicrobial activity, antigen presentation, and inflammatory responses.

The model represents a biologically plausible mechanism supported by the signaling relationships and protein associations investigated in the databases. It should not be interpreted as proof that every step has been experimentally demonstrated in the exact cell pair selected for this activity.

### Interpretation of the Final Model

The proposed communication model shows a possible interaction between a natural killer (NK) cell and a macrophage through interferon-gamma (IFN-γ). The Human Protein Atlas provided RNA expression data for *IFNG* in NK cells, supporting its selection as a candidate signaling molecule. OmniPath displayed an interaction between IFNG and IFNGR1, which helped identify a relevant receptor component for the proposed pathway.

The STRING analysis identified a protein network containing IFNGR1, IFNGR2, JAK1, JAK2, and STAT1. Its functional-enrichment results included the cell surface receptor signaling pathway via JAK-STAT and the type II interferon-mediated signaling pathway. These results are consistent with the proposed mechanism of IFN-γ signaling. IntAct also provided a record reporting a physical association between IFNG and IFNGR1 using a solid phase assay.

Together, the database findings support investigating this signaling pathway as a possible mechanism of communication between NK cells and macrophages. However, expression data and protein associations do not independently establish that the entire pathway occurs in the selected cells under a particular condition. The final model therefore combines database observations with a biologically plausible interpretation of the expected macrophage response.

**Final model figure:** `figures/05_final_model.png`

## 9. References and Database Links

1. **Human Protein Atlas.** IFNG gene expression and single-cell data.  
   https://www.proteinatlas.org/ENSG00000111537-IFNG/single+cell/NK-cells

2. **OmniPath.** A resource for molecular signaling and intercellular communication.  
   https://omnipathdb.org/  
   https://explore.omnipathdb.org/

3. **STRING.** Protein association networks and functional enrichment analysis.  
   https://string-db.org/

4. **IntAct.** Molecular interaction database.  
   https://www.ebi.ac.uk/intact/

5. **UniProt.** Protein sequence and functional information.  
   https://www.uniprot.org/

6. Wojtowicz, W. M., et al. (2020). *A Human IgSF Cell-Surface Interactome Reveals a Complex Network of Protein-Protein Interactions.*  
   PubMed: https://pubmed.ncbi.nlm.nih.gov/32822567/

---

## 10. Conclusion

This activity investigated a proposed cell-to-cell communication pathway involving an NK cell, IFN-γ, and a macrophage. The Human Protein Atlas provided expression data for the candidate ligand, OmniPath helped identify relevant signaling relationships, STRING revealed associated proteins and enriched biological processes, and IntAct provided an experimentally annotated interaction record.

The combined findings support the biological plausibility of IFN-γ-mediated communication and the involvement of JAK–STAT signaling. However, the evidence must be interpreted within the limitations of each database. The proposed model represents an evidence-informed explanation of the pathway rather than proof that the complete signaling sequence occurs in every NK cell and macrophage interaction.
