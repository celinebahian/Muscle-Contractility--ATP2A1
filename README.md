# Muscle-Contractility-ATP2A1

## A

**assignment number:** 23

**gene:** ATP2A1

**transcript:** NM_004320.6

**Matching NP_ protein accession:** NP_004311.1

**ClinVar ID:** 446876

## B. Research question

**1. What does your assigned gene encode, and how does this protein contribute to muscle function?**

- The ATP2A1 gene provides instructions for making a protein called SERCA1, which is found mainly in skeletal muscle cells. This protein helps pump calcium ions back into the sarcoplasmic reticulum after muscle contraction. This lowers the calcium level in the cytoplasm and allows the muscles to relax properly (Molenaar et al., 2020; Velardo et al., 2023).

**2. What was the exact protein accession and length retrieved with R?**

- The protein accession retrieved from NCBI was NP_004311.1, which corresponds to the human ATP2A1 gene and encodes the SERCA1 protein. After analyzing the FASTA file in R, the reference protein sequence was found to contain 994 amino acids.
  
**3. What did the amino-acid composition chart show? What can it NOT tell you?**

- The amino-acid composition chart showed how many times each amino acid appeared in the ATP2A1 protein sequence. Leucine (L) was the most common amino acid, with 97 residues, while Histidine (H) is the least common amino acid, with 9 residues. The chart showed the composition of the reference protein, but it cannot tell us the protein's actual shape, activity, or whether the variant causes a disease.

**4. What is your fixed ClinVar variant, and what is its current classification and evidence strength?**

- My assigned variant is ATP2A1 c.100G>T (p.Glu34Ter), with ClinVar Variation ID 446876. ClinVar currently classifies this variant as pathogenic. Seven of the ten submissions contribute to the aggregate classification, and the record has multiple submitters with no conflicts. The variant has been associated with Brody myopathy, a disorder involving impaired skeletal muscle relaxation (NCBI ClinVar, 2026).

**5. What is the scientifically supported mechanism linking this variant to muscle function, and what remains uncertain?**

- The variant changes the codon at amino acid position 34 into a stop codon. This may cause the protein to be produced in a shortened form or prevent a complete SERCA1 protein from being produced. If SERCA1 function is reduced, calcium may not be transported back into the sarcoplasmic reticulum properly, which can affect muscle relaxation (Molenaar et al., 2020; Velardo et al., 2023). However, my computer analysis cannot confirm whether the altered RNA is degraded, whether a shortened protein is produced, or how much protein activity remains. Laboratory experiments would be needed to confirm the actual effects of this variant.
  
**6. What additional experiment would help test the proposed mechanism?**

- An additional experiment would be to measure SERCA1 ATPase activity or calcium uptake using the normal and variant forms of the protein. The results could show whether the variant affects the protein's ability to transport calcium. Protein expression could also be examined to determine whether the variant produces a shortened protein or reduces protein production. This experiment would help confirm whether the variant affects calcium regulation and muscle relaxation.

## C. Exact numbered methods including R commands

**Step 1. Project Setup**

<img width="522" height="130" alt="image" src="https://github.com/user-attachments/assets/1a41aa2a-f333-45cd-b965-cd420dabba55" />

A project folder named Muscle_Contractility_ATP2A1 was created in RStudio with an R script and separate folders for data, results, and figures. The rentrez and ggplot2 packages were installed and loaded to retrieve information from NCBI and create graphs.

**Step 2. Gene Information Retrieval**

<img width="511" height="515" alt="image" src="https://github.com/user-attachments/assets/68a48ff7-e5bf-472f-801f-8714033c4ebb" />

The ATP2A1 gene was searched in the NCBI database using its gene symbol and the human taxonomy ID. The retrieved gene record was checked, and the gene information was saved as a text file in the results folder.

**Step 3. Protein Sequence Retrieval**

<img width="577" height="324" alt="image" src="https://github.com/user-attachments/assets/38b02687-c727-477c-9eeb-94f68d2f7a80" />

The assigned transcript, NM_004320.6, was used to identify the corresponding protein record in NCBI. The protein sequence was downloaded in FASTA format, saved in the data folder, and its accession number was recorded in the results folder.

**Step 4. Amino Acid Composition Analysis**

<img width="850" height="335" alt="image" src="https://github.com/user-attachments/assets/e0f08a1a-2efc-4767-b645-f87c1e423a3d" />

The downloaded protein sequence was analyzed in R to determine its length and the number of times each amino acid appeared. The amino acid counts were saved as a CSV file, and a bar graph was created to show the amino acid composition of the protein.

**Step 5. ClinVar Variant Examination**

<img width="1353" height="680" alt="image" src="https://github.com/user-attachments/assets/accb877b-f774-40e9-baee-68c1a208fce7" />

ClinVar Variation ID 446876 was examined to collect information about the assigned variant, including its reported classification, associated condition, transcript information, and supporting evidence. The classification and review status were recorded based on the information available on the date the database was accessed.

**Step 6. Protein Variant Visualization**

<img width="658" height="334" alt="image" src="https://github.com/user-attachments/assets/69560a7f-a152-4af4-b0b7-306ca14b4c8d" />

A linear protein map was created using ggplot2 to show the full length of the reference protein and mark the position of p.Glu34Ter at amino acid 34. The figure was saved in the figures folder to show where the assigned variant is located in the protein sequence.

**Step 7. Possible Biological Effects**

The ATP2A1 gene produces a protein called SERCA1, which is mainly found in skeletal muscles. SERCA1 uses energy from ATP to pump calcium ions from the cytoplasm back into the sarcoplasmic reticulum after muscle contraction. This helps lower the calcium level in the cytoplasm and allows the muscles to relax (Molenaar et al., 2020; Velardo et al., 2023). The assigned variant, ATP2A1 c.100G>T (p.Glu34Ter), changes the codon at amino acid position 34 into a stop codon. ClinVar classifies this variant as pathogenic and reports that it may result in an absent or disrupted protein product (NCBI ClinVar, 2026). However, my computer analysis cannot confirm whether the altered RNA is broken down, whether a shortened protein is produced, or how much SERCA1 activity remains. The possible mechanism can be summarized as: ATP2A1 gene → SERCA1 protein → calcium transport for muscle relaxation → p.Glu34Ter variant → possible reduction in SERCA1 production or function → problems with calcium regulation and muscle relaxation. To test this possible effect, a calcium uptake experiment could compare normal SERCA1 with the variant form in a suitable laboratory system. Measuring calcium transport could help determine whether the variant affects the protein's function. Protein expression could also be measured to check whether the variant affects how much protein is produced.

**Step 8. GitHub Repository Preparation**

The R script, protein FASTA file, gene information, protein accession, amino acid composition table, and generated figures were organized into their appropriate folders. A README file was prepared to describe the project, methods, outputs, and biological interpretation.

## D. Results/figures

### Table 1. Amino Acid Composition of the ATP2A1 Reference Protein

| Amino Acid | Count |
|:---:|---:|
| A | 91 |
| C | 24 |
| D | 51 |
| E | 77 |
| F | 36 |
| G | 68 |
| H | 9 |
| I | 70 |
| K | 52 |
| L | 97 |
| M | 29 |
| N | 38 |
| P | 45 |
| Q | 23 |
| R | 49 |
| S | 50 |
| T | 64 |
| V | 85 |
| W | 13 |
| Y | 23 |
| **Total** | **994** |


<img width="2400" height="1500" alt="01_amino_acid_composition" src="https://github.com/user-attachments/assets/05da656e-d545-4a72-acd9-71980031f61d" />

**Figure 1. Amino acid composition of the ATP2A1 reference protein.** Bar graph showing the number of occurrences of each amino acid in the reference protein sequence. The x-axis represents amino acid types, while the y-axis shows the number of residues of each type.pe.


<img width="2400" height="750" alt="02_variant_position" src="https://github.com/user-attachments/assets/b703d280-59f9-477e-9297-6417fe5634a8" />

**Figure 2. Protein variant position in ATP2A1.** Linear map of the reference protein showing the location corresponding to the p.Glu34Ter variant at amino acid position 34. This marks the variant position; it does not demonstrate that a shortened protein was actually produced.

## E. Variant interpretation

- The assigned variant in the *ATP2A1* gene is c.100G>T (p.Glu34Ter), recorded in ClinVar under Variation ID 446876 (NCBI ClinVar, 2026). This is a nonsense, or stop-gain, variant because the nucleotide substitution changes the codon for glutamic acid at amino acid position 34 into a premature stop codon. ClinVar classifies this variant as pathogenic and reports that it is expected to result in an absent or disrupted protein product (NCBI ClinVar, 2026). The *ATP2A1* gene encodes SERCA1, a calcium pump found mainly in skeletal muscle cells that transports calcium ions back into the sarcoplasmic reticulum after muscle contraction. This process is important for normal muscle relaxation (Molenaar et al., 2020; Velardo et al., 2023). If the variant reduces SERCA1 production or function, calcium regulation in skeletal muscle cells may be disrupted, potentially contributing to the impaired muscle relaxation associated with Brody myopathy (Molenaar et al., 2020; NCBI ClinVar, 2026). However, sequence analysis alone cannot confirm whether the altered RNA is degraded, whether a shortened protein is produced, or how much SERCA1 activity remains. Further laboratory studies would be needed to investigate its specific molecular effects.

## F. Limitations and a possible validation experiment

- One limitation of this analysis is that it mainly uses information from online databases and computer-based protein sequence analysis. These methods can identify the variant's location and predict its possible effect, but they cannot directly confirm whether the variant changes protein expression, stability, or activity. The analysis also depends on the accuracy and completeness of the available database records. A possible validation experiment would be to measure SERCA1 ATPase activity or calcium uptake in an appropriate experimental system containing the reference and variant forms of the protein. The results could be compared to determine whether the variant affects calcium transport activity. Protein expression could also be examined to investigate whether the variant changes the amount or stability of the protein. These experiments would require suitable laboratory facilities and controls. Until experimental results are available, the predicted effects should be treated as possibilities rather than confirmed findings.

## G. Database links, accession versions, access dates, and citations.

| Database/Resource | Accession or Record ID | Link | Access Date |
|---|---|---|---|
| NCBI Gene | ATP2A1 (Human) | [NCBI Gene](https://www.ncbi.nlm.nih.gov/gene/?term=ATP2A1%5BGene%20Name%5D%20AND%20Homo%20sapiens%5BOrganism%5D) | October 27, 2026 |
| NCBI Nucleotide | NM_004320.6 | [NCBI Nucleotide](https://www.ncbi.nlm.nih.gov/nuccore/NM_004320.6) | October 27, 2026 |
| NCBI Protein | NP_004311.1 | [NCBI Protein](https://www.ncbi.nlm.nih.gov/protein/NP_004311.1) | October 27, 2026 |
| ClinVar | Variation ID 446876 | [ClinVar](https://www.ncbi.nlm.nih.gov/clinvar/variation/446876/) | October 27, 2026 |
| R Project | R statistical software | [R Project](https://www.r-project.org/) | October 27, 2026 |

## H. Discussion

The ATP2A1 gene produces a protein called SERCA1, which is mainly found in skeletal muscles. SERCA1 uses energy from ATP to move calcium ions from the cytoplasm back into the sarcoplasmic reticulum after muscle contraction. This process helps muscles relax properly (Molenaar et al., 2020; Velardo et al., 2023). When SERCA1 activity is reduced, calcium regulation may be affected, making muscle relaxation more difficult.

The assigned variant, ATP2A1 c.100G>T (p.Glu34Ter), changes the codon for glutamic acid at position 34 into a stop codon. ClinVar classifies this variant as pathogenic and reports its association with Brody myopathy (NCBI ClinVar, 2026). This clinical information supports a link between the variant and the disease. However, the classification alone does not explain exactly how the variant affects the protein.

Experimental research has found lower SERCA activity in muscle samples from people with Brody disease than in healthy individuals. The study also included a person with two copies of the p.Glu34Ter variant. This finding supports the possibility that the variant is related to reduced SERCA activity. However, because the researchers measured activity in muscle samples, the results do not show the exact effect of the variant on the SERCA1 protein by itself.

Based on the DNA change, the variant is predicted to stop protein production too early. This could prevent the production of a complete SERCA1 protein or cause the altered RNA to break down. ClinVar also mentions a possible effect on RNA splicing. However, these specific effects were not tested in my computer analysis, so they cannot be confirmed by this project alone.

A follow-up experiment could compare calcium uptake by normal SERCA1 and the variant form in a suitable laboratory system. Protein levels could also be measured to determine whether the variant affects protein production. Overall, the clinical information and experimental findings support the possibility that this variant reduces SERCA1 function. Further experiments are needed to confirm the exact molecular effects of the variant.

### Scientific References

Molenaar, J. P., et al. (2020). Clinical, morphological and genetic characterization of Brody disease: An international study of 40 patients. *Brain, 143*(2), 452–466. https://doi.org/10.1093/brain/awz410

Molenaar, J. P., Snoeck, M. M., Treves, S., Stoltenborg, B. J., Wethly, K. C., Oosterhof, A., Kamsteeg, E. J., Sternberg, D., Doorduin, J., van Engelen, B. G., Voermans, N. C., & Rodenburg, R. J. (2026). Sarco/endoplasmatic reticulum calcium ATPase activity in healthy muscle and Brody disease. Biochemistry and Biophysics Reports, 46, 102554. https://doi.org/10.1016/j.bbrep.2026.102554 https://pmc.ncbi.nlm.nih.gov/articles/PMC13050089/?utm_source=chatgpt.com

National Center for Biotechnology Information. (2026). NM_004320.6(ATP2A1):c.100G>T (p.Glu34Ter) (ClinVar Variation ID 446876). https://www.ncbi.nlm.nih.gov/clinvar/variation/446876/

Velardo, D., Antognozzi, S., Rimoldi, M., Pagliarani, S., Cogiamanian, F., Barbieri, S., Corti, S., Comi, G. P., & Ronchi, D. (2023). Case report: Clinical and molecular characterization of two siblings affected by Brody myopathy. *Frontiers in Neurology, 14*, 1170071. https://doi.org/10.3389/fneur.2023.1170071
