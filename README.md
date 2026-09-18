# From Gene Mutation to Disease: GALT Mutation Analysis in Classic Galactosemia

**Student:** Shahanta Dawn B. Balanza  
**Disease:** Classic Galactosemia  
**Gene:** GALT  
**Documented Variant:** NM_000155.4:c.563A>G (p.Gln188Arg)
**Reference Transcript Accession:** NM_000155.4  
**Reference Protein Accession:** NP_000146.2  
**ClinVar Accession:** RCV000825563.20  
**Galaxy History Name:** Balanza_Galactosemia_GALT_Mutation_Lab  
**Date of Analysis:** September 16, 2026

## Project Overview

This repository contains the sequence analysis and documentation for a Cell and Molecular Biology Laboratory activity investigating how a DNA mutation can affect a protein product and contribute to a disease phenotype.

The project focuses on the **GALT** gene and the documented **c.563A>G (p.Gln188Arg/Q188R)** variant associated with classic galactosemia.

## Objectives

This project was conducted to:

- Identify a documented disease-associated mutation in the GALT gene.
- Establish the normal GALT sequence as the wild-type (WT) control.
- Translate the WT coding sequence and examine its predicted protein product.
- Reproduce the documented c.563A>G mutation using Galaxy.
- Compare the WT and documented mutant protein sequences.
- Create an artificial synonymous mutation for comparison.
- Interpret how nucleotide changes can affect protein products and disease-related molecular function.

## Reference Sequences

The WT GALT coding sequence was obtained from the NCBI RefSeq transcript **NM_000155.4**.

**Reference protein:** NP_000146.2

The WT CDS is **1,140 bp** and produces a predicted GALT protein of **379 amino acids**.

## Documented Mutation

**Variant:** NM_000155.4:c.563A>G (p.Gln188Arg)

The nucleotide substitution changes **A → G** at coding position 563. This changes the codon from **CAG → CGG**, resulting in the amino-acid substitution **Q → R at position 188**.

The mutation is a **missense variant**.

## Artificial Mutation

An artificial synonymous mutation, **c.564G>A**, was introduced into a separate copy of the WT CDS.

This changes:

**CAG → CAA**

Both codons encode glutamine (Q), so the predicted protein sequence remains unchanged.

## Repository Structure

```text
Balanza_Galactosemia_GALT_Mutation_Lab/
│
├── 01_reference/
│   ├── GALT_WT_CDS.fasta
│   └── GALT_WT_protein.fasta
│
├── 02_documented_mutation/
│   ├── GALT_c.563A>G_mutant_CDS.fasta
│   └── GALT_c.563A>G_mutant_protein.fasta
│
├── 03_artificial_mutation/
│   ├── GALT_artificial_synonymous_mutant_CDS.fasta
│   └── GALT_artificial_synonymous_mutant_protein.fasta
│
├── 04_results/
│   ├── WT_vs_mutant_alignment.txt
│   └── results_summary.md
│
├── 05_report/
│   └── final_report.md
│
├── disease_gene_background.md
└── README.md
```

## Main Results

The documented **c.563A>G** mutation produced the predicted protein change **p.Gln188Arg (Q188R)**.

The WT and documented mutant proteins were both **379 amino acids** long. The documented mutant differed from the WT at amino-acid position **188**, with **Q replaced by R**.

No frameshift, insertion, deletion, or premature stop codon was observed.

The artificial **c.564G>A** mutation produced no amino-acid change, demonstrating a synonymous substitution.

## Tools Used

- **NCBI RefSeq** — reference GALT sequence
- **NCBI ClinVar** — documented variant information
- **Galaxy** — sequence processing and translation
- **SeqKit Translate** — translation of CDS sequences
- **GitHub** — project organization and documentation

## GitHub Documentation

The repository contains the reference sequences, documented and artificial mutation sequences, protein comparisons, results summary, and final report used for the laboratory activity.

## Final Report

The complete GitHub final report is available in:

**`05_report/final_report.md`**

## References

- Berry, G. T. (2021). Classic galactosemia and clinical variant galactosemia. In *GeneReviews®*. University of Washington, Seattle.
- Elsevier, J. P., & Fridovich-Keil, J. L. (1996). The Q188R mutation in human galactose-1-phosphate uridylyltransferase acts as a partial dominant negative. *Journal of Biological Chemistry, 271*(50), 32002–32007.
- McCorvie, T. J., & Timson, D. J. (2011). Structural and molecular biology of type I galactosemia: Disease-associated mutations. *IUBMB Life, 63*(11), 949–954.
- McCorvie, T. J., Kopec, J., Pey, A. L., Shrestha, L., Yue, W. W., & Timson, D. J. (2016). Molecular basis of classic galactosemia from the structure of human galactose 1-phosphate uridylyltransferase. *Human Molecular Genetics, 25*(11), 2234–2244.
- NCBI ClinVar. GALT c.563A>G (p.Gln188Arg), Variation ID 3614.
- NCBI RefSeq. *GALT* transcript NM_000155.4 and protein NP_000146.2.
