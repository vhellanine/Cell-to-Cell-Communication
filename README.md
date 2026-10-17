# Cell-to-Cell Communication Laboratory: IFN-γ Signaling

## Student Information
- **Student Name:** Junavhel Jane B. Olaguir
- **Course/Section:** BS Biology – [Insert Section]
- **Organism:** *Homo sapiens*
- **Chosen Sender Cell:** Natural Killer (NK) Cell
- **Receiver Cell:** Macrophage

---
## Biological Question

How can natural killer (NK) cells communicate with macrophages through IFN-γ signaling during immune activation?

## Chosen Sender Cell and Biological Context

| Item | Answer |
|---|---|
| Sender cell | Natural Killer (NK) cell |
| Biological context | Immune activation / immune regulation |
| Main purpose | Communication between immune cells through a secreted cytokine |
| Receiver cell | Macrophage |

## Candidate Ligand and Evidence for Sender-Cell Expression

| Item | Information |
|---|---|
| Sender cell | Natural Killer (NK) cell |
| Candidate ligand | IFN-γ |
| Gene | IFNG |
| Protein name | Interferon-gamma |
| Predicted location | Secreted cytokine |
| Expression evidence | The Human Protein Atlas (HPA) provides IFNG RNA expression data for NK cells. |
| HPA expression value | 0.9 nTPM |
| Monaco dataset | 57.4 nTPM |
| Schmiedel dataset | 134.6 TPM |
| Supporting database | Human Protein Atlas |

The HPA results support investigating IFN-γ as a candidate signal produced by NK cells. The expression values differ across datasets, so they should be interpreted according to their respective data sources. RNA expression alone does not prove that IFN-γ was secreted under a particular condition.

## Receptor and Receiver Cell with Supporting Evidence

| Item | Information |
|---|---|
| Ligand | IFN-γ |
| Receptor | IFNGR1 and IFNGR2 |
| Receiver cell | Macrophage |
| Receptor protein | Interferon-gamma receptor subunits 1 and 2 |
| Receptor localization | Cell membrane |
| Signaling context | Immune activation and regulation |
| Supporting databases | Human Protein Atlas and OmniPath |

The proposed receiver cell is a macrophage because macrophages can respond to IFN-γ through the IFN-γ receptor complex, which consists of IFNGR1 and IFNGR2. Additional receiver-cell expression evidence can help establish the relevance of this receptor in the selected biological context.

## OmniPath Findings

| Component | Gene | Finding |
|---|---|---|
| Ligand | IFNG | Candidate secreted signaling molecule |
| Receptor | IFNGR1 | IFNG-to-IFNGR1 interaction displayed |
| Receptor subunit | IFNGR2 | Investigated as the second receptor component |
| Signaling protein | STAT1 | Association involving IFNG and STAT1 displayed |
| Supporting database | — | OmniPath |

OmniPath displayed an interaction from IFNG to IFNGR1, supporting further investigation of this receptor component. STAT1 also appeared in the results, but this association should not be interpreted as direct binding between IFN-γ and STAT1. The findings provide evidence of annotated signaling relationships rather than proof of the complete pathway in the selected cells.

## STRING Network Interpretation

The STRING network contained **11 nodes and 55 edges**, compared with 16 expected edges. The reported PPI enrichment p-value was **8.76 × 10⁻¹⁵**.

Relevant proteins identified in the network include:

- IFNGR1
- IFNGR2
- JAK1
- JAK2
- STAT1

Other proteins displayed included STAT3, SOCS1, and TYK2.

The network showed significant functional enrichment. Relevant biological processes included:

| Enriched biological process | False discovery rate |
|---|---:|
| Type II interferon-mediated signaling pathway | 1.53 × 10⁻¹⁷ |
| Cell surface receptor signaling pathway via JAK-STAT | 6.89 × 10⁻¹⁸ |
| Interferon-mediated signaling pathway | 8.76 × 10⁻¹⁸ |
| Cellular response to virus | 1.40 × 10⁻¹⁴ |
| Type III interferon-mediated signaling pathway | 5.27 × 10⁻¹² |

The cell surface receptor signaling pathway via JAK-STAT is particularly relevant to the proposed mechanism. IFNGR1 and IFNGR2 form the receptor complex, JAK1 and JAK2 participate in intracellular signaling, and STAT1 regulates downstream gene expression.

These findings are consistent with interferon-mediated signaling and immune regulation. However, STRING represents functional protein associations and does not automatically establish direct physical binding or the direction of every interaction.

## IntAct Validation

| Item | Information |
|---|---|
| Protein pair examined | IFNG – IFNGR1 |
| IntAct accession | EBI-64053318 |
| Organism | Homo sapiens |
| Host organism | In vitro |
| Interaction type | Physical association |
| Detection method | Solid phase assay |
| Positive interaction | Yes |
| Publication PMID | 32822567 |
| Publication | A Human IgSF Cell-Surface Interactome Reveals a Complex Network of Protein-Protein Interactions |

The IntAct record reports a positive physical association between IFNG and IFNGR1 using a solid phase assay. This is relevant to the proposed ligand–receptor relationship. However, the record must be interpreted in the context of the reported experiment and does not independently prove the complete signaling pathway in the selected NK cell and macrophage pair.

## Interaction Summary

The interaction summary file records selected protein pairs, the database in which each result was observed, the reported result, and the available supporting evidence.

**File:** [`data/interaction_summary.csv`](data/interaction_summary.csv)

| Protein A | Protein B | Database | Result |
|---|---|---|---|
| IFNG | IFNGR1 | OmniPath | Interaction displayed |
| IFNG | IFNGR1 | IntAct | Physical association supported |
| IFNGR1 | IFNGR2 | IntAct | Specific interaction not confirmed |
| IFNGR1 | JAK1 | STRING | Protein association shown |
| IFNGR2 | JAK2 | STRING | Protein association shown |
| JAK1 | STAT1 | STRING | Protein association shown |

The summary distinguishes the interaction evidence reported by each database. STRING associations are not necessarily direct physical interactions, and the IFNGR1–IFNGR2 IntAct interaction was not confirmed in the screenshots examined.

## Final Model

The proposed signaling sequence is:

**NK cell → IFN-γ → IFNGR1/IFNGR2 → JAK1/JAK2 → STAT1 → Macrophage response**

### Final IFN-γ Cell-to-Cell Communication Model

**Figure 1.** Proposed IFN-γ cell-to-cell communication model showing the NK cell as the sender, secretion of IFN-γ into the extracellular space, the IFNGR1/IFNGR2 receptor complex on the macrophage, downstream JAK–STAT signaling, and the potential cellular response.

![Final IFN-gamma cell-to-cell communication model](figures/05_final_model.png)

## Interpretation

My proposed model shows communication between a natural killer (NK) cell and a macrophage through interferon-gamma (IFN-γ). The Human Protein Atlas provides IFNG expression data for NK cells, supporting its selection as a candidate signaling molecule. However, the reported values differ across datasets, and RNA expression alone does not demonstrate cytokine secretion. OmniPath displayed an interaction between IFNG and IFNGR1, which supports investigating IFNGR1 as part of the receptor for this signal.

The STRING network contained IFNGR1, IFNGR2, JAK1, JAK2, and STAT1. Its enrichment results included the cell surface receptor signaling pathway via JAK-STAT and the type II interferon-mediated signaling pathway. IntAct also provided a record reporting a physical association between IFNG and IFNGR1 using a solid phase assay. Together, these results support the biological plausibility of the proposed signaling mechanism.

However, the databases do not independently demonstrate the complete communication pathway between the exact NK cell and macrophage selected for this activity. The resulting macrophage response is therefore a proposed biological interpretation supported by the available database evidence.

## Questions and Answers

### 1. What sender cell did you choose, and in what tissue or biological context does it act?

I chose the natural killer (NK) cell as my sender cell. NK cells are part of the innate immune system and participate in immune defense. I selected immune activation and communication with macrophages as the biological context because NK cells can release cytokines that influence other immune cells.

### 2. What signaling molecule did you identify, and what evidence supports its production or presentation by the sender cell?

I identified interferon-gamma (IFN-γ), encoded by the IFNG gene, as my candidate signaling molecule. The Human Protein Atlas provides RNA expression data for IFNG in NK cells. The reported values vary across the HPA, Monaco, and Schmiedel datasets. These findings support investigating IFN-γ as a candidate signal, although RNA expression alone does not establish secretion.

### 3. What receptor receives the signal, and which receiver cell did you select?

I selected IFNGR1 and IFNGR2 as the receptor subunits and macrophage as the receiver cell. OmniPath displayed an interaction from IFNG to IFNGR1. Macrophages can respond to IFN-γ through its receptor complex, making them a reasonable receiver-cell choice for this proposed model.

### 4. What type of cell-to-cell signaling is represented: paracrine, endocrine, autocrine, or contact-dependent?

I classified the proposed interaction as paracrine signaling because IFN-γ is a secreted cytokine that can act on another cell. In this model, the NK cell releases IFN-γ, which can bind to receptors on a macrophage. The specific communication event remains a proposed interpretation of the available evidence.

### 5. Which proteins in your STRING network appear most relevant to the receptor-associated response? Explain briefly.

The proteins I considered most relevant are IFNGR1, IFNGR2, JAK1, JAK2, and STAT1. IFNGR1 and IFNGR2 form the receptor complex, JAK1 and JAK2 participate in intracellular signaling, and STAT1 regulates downstream gene expression. These proteins provide a plausible connection between receptor activation and the macrophage response.

### 6. What enriched pathway or biological process is consistent with your proposed mechanism?

The STRING analysis showed enrichment for the cell surface receptor signaling pathway via JAK-STAT and the type II interferon-mediated signaling pathway. Their false discovery rates were 6.89 × 10⁻¹⁸ and 1.53 × 10⁻¹⁷, respectively. These processes are consistent with the proposed IFN-γ signaling mechanism and its role in immune regulation.

### 7. What did IntAct show for the molecular interaction you examined? What type of evidence was reported?

I examined the IFNG–IFNGR1 interaction in IntAct. The record, EBI-64053318, reported a positive physical association detected using a solid phase assay. The associated publication had PMID 32822567. This supports an association under the reported experimental conditions but does not independently prove the complete signaling pathway in the selected cells.

### 8. Which parts of your final model are strongly supported, and which parts remain an inference?

The database results support investigating IFN-γ as a candidate NK-cell signal, IFNGR1 as a receptor component, and JAK–STAT signaling as a relevant pathway. STRING enrichment and the IntAct interaction record provide additional supporting evidence. However, the exact communication between the selected NK cell and macrophage, the complete signaling sequence, and the resulting response remain biological inferences.

### 9. What cellular response is expected in the receiver cell, and why?

The expected response is macrophage activation and changes in gene expression related to immune regulation and cellular defense. This is proposed because IFN-γ can signal through IFNGR1/IFNGR2 and activate the JAK–STAT pathway. The specific response depends on the macrophage's condition and biological environment.

## References and Database Links

1. Human Protein Atlas: https://www.proteinatlas.org/
2. HPA IFNG single-cell expression page: https://www.proteinatlas.org/ENSG00000111537-IFNG/single+cell/NK-cells
3. OmniPath: https://omnipathdb.org/
4. OmniPath Explorer: https://explore.omnipathdb.org/
5. STRING: https://string-db.org/
6. IntAct: https://www.ebi.ac.uk/intact/
7. UniProt: https://www.uniprot.org/
8. PubMed, PMID 32822567: https://pubmed.ncbi.nlm.nih.gov/32822567/
