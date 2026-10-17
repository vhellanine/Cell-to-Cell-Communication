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
| Biological context | Immune activation and immune regulation |
| Main purpose | Communication between immune cells through a secreted cytokine |
| Receiver cell | Macrophage |

## Candidate Ligand and Evidence for Sender-Cell Expression

| Item | Information |
|---|---|
| Sender cell | Natural Killer (NK) cell |
| Candidate ligand | IFN-γ |
| Gene | *IFNG* |
| Protein name | Interferon-gamma |
| Predicted location | Secreted cytokine |
| Expression evidence | The Human Protein Atlas (HPA) provides *IFNG* RNA expression data for NK cells. |
| HPA expression value | 0.9 nTPM |
| Monaco dataset | 57.4 nTPM |
| Schmiedel dataset | 134.6 TPM |
| Supporting database | Human Protein Atlas |

The HPA results support investigating IFN-γ as a candidate signaling molecule produced by NK cells. However, the reported expression levels differ across datasets, and RNA expression alone does not establish that the cytokine was secreted under a particular condition.

## Receptor and Receiver Cell with Supporting Evidence

| Item | Information |
|---|---|
| Ligand | IFN-γ |
| Ligand gene | *IFNG* |
| Receptor | IFNGR1 and IFNGR2 |
| Receptor name | Interferon-gamma receptor subunits 1 and 2 |
| Receiver cell | Macrophage |
| Receptor localization | Cell membrane |
| Signaling context | Immune activation and regulation |
| Supporting databases | Human Protein Atlas and OmniPath |

The proposed receiver cell is a macrophage because macrophages can respond to IFN-γ through the IFN-γ receptor complex. The receptor consists of IFNGR1 and IFNGR2. Additional expression evidence should be used to establish the receptor's relevance to the selected receiver cell.

## OmniPath Findings

| Component | Gene | Finding |
|---|---|---|
| Ligand | *IFNG* | Candidate secreted signaling molecule |
| Receptor component | *IFNGR1* | An IFNG-to-IFNGR1 interaction was displayed in the search results |
| Receptor component | *IFNGR2* | Investigated as the second receptor subunit |
| Signaling protein | *STAT1* | An association involving IFNG and STAT1 appeared in the results |
| Additional proteins | *TBX21*, *RELB* | Also displayed among the signaling-related results |
| Supporting database | — | OmniPath |

OmniPath supports investigating IFN-γ and IFNGR1 as components of the proposed signaling pathway. The displayed association involving STAT1 is relevant to the investigation, but it does not establish that IFN-γ directly binds STAT1. The database results must be interpreted as annotated signaling information rather than proof that the complete pathway occurs in the selected cells.

## STRING Network Interpretation

The STRING network contained **11 nodes and 55 edges**, compared with 16 expected edges. The reported PPI enrichment p-value was **8.76 × 10⁻¹⁵**.

Relevant proteins identified in the network include:

- IFNGR1
- IFNGR2
- JAK1
- JAK2
- STAT1

Other proteins displayed in the network included STAT3, SOCS1, and TYK2.

The functional-enrichment results included the following biological processes:

| Enriched biological process | False discovery rate |
|---|---:|
| Type II interferon-mediated signaling pathway | 1.53 × 10⁻¹⁷ |
| Cell surface receptor signaling pathway via JAK-STAT | 6.89 × 10⁻¹⁸ |
| Interferon-mediated signaling pathway | 8.76 × 10⁻¹⁸ |
| Cellular response to virus | 1.40 × 10⁻¹⁴ |
| Type III interferon-mediated signaling pathway | 5.27 × 10⁻¹² |

The cell surface receptor signaling pathway via JAK-STAT is particularly relevant to the proposed mechanism. IFNGR1 and IFNGR2 form the receptor complex, JAK1 and JAK2 participate in intracellular signaling, and STAT1 regulates downstream gene expression.

These findings are consistent with interferon-mediated signaling and immune regulation. However, STRING represents functional protein associations and does not automatically demonstrate direct physical binding or establish the direction of every interaction.

## IntAct Validation

| Item | Information |
|---|---|
| Protein pair examined | IFNG – IFNGR1 |
| IntAct accession | EBI-64053318 |
| Organism | *Homo sapiens* |
| Host organism | In vitro |
| Interaction type | Physical association |
| Detection method | Solid phase assay |
| Positive interaction | Yes |
| Publication PMID | 32822567 |
| Publication | *A Human IgSF Cell-Surface Interactome Reveals a Complex Network of Protein-Protein Interactions* |

The IntAct record reports a positive physical association between IFNG and IFNGR1, detected using a solid phase assay. This evidence is relevant to the proposed ligand–receptor relationship.

However, the experimental context must be considered. The record alone does not establish that the interaction occurs under every physiological condition or prove the complete IFN-γ signaling pathway in the selected NK cell and macrophage pair.

## Final Model

The proposed signaling sequence is:

**NK cell → IFN-γ → IFNGR1/IFNGR2 → JAK1/JAK2 → STAT1 → Macrophage response**

### Final IFN-γ Cell-to-Cell Communication Model

**Figure 1.** Proposed IFN-γ cell-to-cell communication model showing the NK cell as the sender, the release of IFN-γ into the extracellular space, the IFNGR1/IFNGR2 receptor complex on the macrophage, downstream JAK–STAT signaling, and the potential cellular response.

### Interpretation

My proposed model shows communication between a natural killer (NK) cell and a macrophage through interferon-gamma (IFN-γ). The Human Protein Atlas provides *IFNG* expression data for NK cells, supporting its selection as a candidate signaling molecule. However, the reported expression values vary across datasets, so RNA expression alone does not establish cytokine secretion. OmniPath displayed an interaction between IFNG and IFNGR1, which supports investigating IFNGR1 as part of the receptor for this signaling molecule.

The STRING network contained IFNGR1, IFNGR2, JAK1, JAK2, and STAT1. Its enrichment results included the cell surface receptor signaling pathway via JAK-STAT and the type II interferon-mediated signaling pathway, consistent with the proposed mechanism. IntAct also reported a physical association between IFNG and IFNGR1 detected using a solid phase assay. This provides relevant interaction evidence, although the experimental context must be considered.

Overall, the database findings support the biological plausibility of IFN-γ-mediated communication and the involvement of JAK–STAT signaling. However, the specific communication between the selected NK cell and macrophage, along with the complete sequence of intracellular events and resulting response, remains a proposed biological interpretation rather than a fully demonstrated mechanism.

## Questions and Answers

### 1. What sender cell did you choose, and in what tissue or biological context does it act?

I chose the natural killer (NK) cell as my sender cell. NK cells are part of the innate immune system and participate in immune defense. I selected immune activation and communication with macrophages as the biological context because NK cells can produce cytokines that influence other immune cells.

### 2. What signaling molecule did you identify, and what evidence supports its production or presentation by the sender cell?

I identified interferon-gamma (IFN-γ), encoded by the *IFNG* gene, as my candidate signaling molecule. The Human Protein Atlas provides RNA expression data for *IFNG* in NK cells. The HPA, Monaco, and Schmiedel datasets reported different expression values, supporting further investigation of IFN-γ while showing that expression varies across datasets. These results do not independently prove that the cytokine was secreted.

### 3. What receptor receives the signal, and which receiver cell did you select?

I selected IFNGR1 and IFNGR2 as the receptor subunits and macrophage as the receiver cell. OmniPath displayed an interaction from IFNG to IFNGR1. IFN-γ signaling through the receptor complex is biologically consistent with macrophage immune responses, although receptor-expression evidence should also be considered for the selected receiver cell.

### 4. What type of cell-to-cell signaling is represented: paracrine, endocrine, autocrine, or contact-dependent?

I classified the proposed interaction as paracrine signaling because IFN-γ is a secreted cytokine that can act on another cell. In this model, the NK cell releases IFN-γ, which can bind to receptors on a macrophage. The specific communication between these selected cells remains an inference based on the available evidence.

### 5. Which proteins in your STRING network appear most relevant to the receptor-associated response? Explain briefly.

The proteins I considered most relevant are IFNGR1, IFNGR2, JAK1, JAK2, and STAT1. IFNGR1 and IFNGR2 form the receptor complex, JAK1 and JAK2 participate in intracellular signaling, and STAT1 regulates downstream gene expression. Together, these proteins provide a plausible connection between receptor activation and a cellular response.

### 6. What enriched pathway or biological process is consistent with your proposed mechanism?

The STRING results included the cell surface receptor signaling pathway via JAK-STAT and the type II interferon-mediated signaling pathway. Their false discovery rates were 6.89 × 10⁻¹⁸ and 1.53 × 10⁻¹⁷, respectively. These enriched processes are consistent with the proposed IFN-γ signaling mechanism and its role in immune regulation.

### 7. What did IntAct show for the molecular interaction you examined? What type of evidence was reported?

I examined the IFNG–IFNGR1 interaction in IntAct. The record, EBI-64053318, reported a positive physical association detected using a solid phase assay. The associated publication had PMID 32822567. This supports a physical association under the reported experimental conditions but does not independently prove the complete signaling pathway in the proposed cell pair.

### 8. Which parts of your final model are strongly supported, and which parts remain an inference?

The database findings support investigating IFN-γ as a candidate NK-cell signal, IFNGR1 as a receptor component, and JAK–STAT signaling as a relevant pathway. STRING enrichment and the IntAct interaction record provide additional support for the proposed mechanism. However, the exact NK cell-to-macrophage communication event, the complete sequence of intracellular signaling, and the resulting response in the selected cells remain biological inferences.

### 9. What cellular response is expected in the receiver cell, and why?

The expected response is macrophage activation and changes in gene expression related to immune regulation and cellular defense. This is proposed because IFN-γ can signal through IFNGR1/IFNGR2 and activate the JAK–STAT pathway. The specific response depends on the macrophage's condition and the surrounding biological environment.

## References and Database Links

1. Human Protein Atlas: https://www.proteinatlas.org/
2. IFNG single-cell expression page: https://www.proteinatlas.org/ENSG00000111537-IFNG/single+cell/NK-cells
3. OmniPath: https://omnipathdb.org/
4. OmniPath Explorer: https://explore.omnipathdb.org/
5. STRING: https://string-db.org/
6. IntAct: https://www.ebi.ac.uk/intact/
7. UniProt: https://www.uniprot.org/
8. PubMed, PMID 32822567: https://pubmed.ncbi.nlm.nih.gov/32822567/
