# Muscle-Contractility--ATP2A1

## A
**assignment number:** 23

**gene:** ATP2A1

**transcript:** NM_004320.6

**Matching NP_ protein accession:** NP_004311.1

**ClinVar ID:** 446876

## B. Research question

**1. What does your assigned gene encode, and how does this protein contribute to muscle function?**

**2. What was the exact protein accession and length retrieved with R?**

**3. What did the amino-acid composition chart show? What can it NOT tell you?**

**4. What is your fixed ClinVar variant, and what is its current classification and evidence strength?5. What is the scientifically supported mechanism linking this variant to muscle function, and what remains uncertain?**

**6. What additional experiment would help test the proposed mechanism?**

## C. Exact numbered methods including R commands

**Step 1. Project Setup**

A project folder named Muscle_Contractility_ATP2A1 was created in RStudio with an R script and separate folders for data, results, and figures. The rentrez and ggplot2 packages were installed and loaded to retrieve information from NCBI and create graphs.

**Step 2. Gene Information Retrieval**

The ATP2A1 gene was searched in the NCBI database using its gene symbol and the human taxonomy ID. The retrieved gene record was checked, and the gene information was saved as a text file in the results folder.

**Step 3. Protein Sequence Retrieval**

The assigned transcript, NM_004320.6, was used to identify the corresponding protein record in NCBI. The protein sequence was downloaded in FASTA format, saved in the data folder, and its accession number was recorded in the results folder.

**Step 4. Amino Acid Composition Analysis**

The downloaded protein sequence was analyzed in R to determine its length and the number of times each amino acid appeared. The amino acid counts were saved as a CSV file, and a bar graph was created to show the amino acid composition of the protein.

**Step 5. ClinVar Variant Examination**

ClinVar Variation ID 446876 was examined to collect information about the assigned variant, including its reported classification, associated condition, transcript information, and supporting evidence. The classification and review status were recorded based on the information available on the date the database was accessed.

**Step 6. Protein Variant Visualization**

A linear protein map was created using ggplot2 to show the full length of the reference protein and mark the position of p.Glu34Ter at amino acid 34. The figure was saved in the figures folder to show where the assigned variant is located in the protein sequence.

## D. Results/figures

## E. Variant interpretation

## F. Limitations and a possible validation experiment

## G. Database links, accessionversions, access dates, and citations.
