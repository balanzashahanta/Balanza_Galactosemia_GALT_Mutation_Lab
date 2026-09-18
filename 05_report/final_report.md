# From Gene Mutation to Disease: Investigating How DNA Sequence Changes Affect Protein Products and Human Phenotypes

**Student:** Shahanta Dawn B. Balanza  
**Disease:** Classic Galactosemia  
**Gene:** GALT  
**Documented Variant:** NM_000155.4:c.563A>G (p.Gln188Arg)

## Disease Background

Classic galactosemia is an inherited disorder of galactose metabolism caused by pathogenic variants in the **GALT** gene. These variants reduce the activity of galactose-1-phosphate uridylyltransferase, an enzyme involved in the Leloir pathway of galactose metabolism. Reduced GALT activity can lead to the accumulation of galactose-1-phosphate and other galactose metabolites, contributing to clinical manifestations that may affect multiple tissues and organs.

## Gene and Normal Protein Function

The **GALT** gene encodes the enzyme **galactose-1-phosphate uridylyltransferase**. The gene is located on chromosome **9p13.3**. GALT functions in the cytosol as part of the Leloir pathway.

The GALT enzyme catalyzes the conversion of **galactose-1-phosphate and UDP-glucose into UDP-galactose and glucose-1-phosphate**. This reaction is important for the normal metabolism of galactose and the processing of galactose-containing compounds.

## Documented Mutation

The documented disease-associated variant investigated in this experiment was **NM_000155.4:c.563A>G (p.Gln188Arg)**, also known as **Q188R**.

The mutation is a single-nucleotide substitution in the GALT coding sequence. The change from **A to G at nucleotide position 563** changes the codon from **CAG to CGG**, resulting in the replacement of **glutamine (Q) with arginine (R) at amino-acid position 188**. Therefore, the variant is classified as a **missense mutation**.

ClinVar classifies this variant as pathogenic for galactosemia. Published studies have also reported reduced GALT enzyme activity associated with the Q188R variant.

## Hypothesis

Before constructing the documented mutation, it was hypothesized that changing nucleotide **563 from A to G** would change the encoded amino acid at position **188 from glutamine (Q) to arginine (R)**. Because the mutation is a single-nucleotide substitution rather than an insertion or deletion, the reading frame and overall protein length were expected to remain unchanged. No premature stop codon was expected.

## Methods

The normal GALT coding sequence was obtained from the NCBI RefSeq transcript **NM_000155.4**, with the corresponding reference protein **NP_000146.2**. The WT CDS was uploaded to Galaxy as the reference sequence.

The WT CDS was translated using **SeqKit Translate** with the standard genetic code and reading frame 1. The resulting WT protein sequence was saved for comparison with the reference protein.

A copy of the WT CDS was then used to reproduce the documented **c.563A>G** mutation. Nucleotide position 563 was manually changed from **A to G** using the Galaxy sequence editor. The modified CDS was exported and translated using the same SeqKit settings.

A separate copy of the WT CDS was used to create an artificial synonymous mutation, **c.564G>A**. This changed the codon from **CAG to CAA**. The artificial mutant CDS was also translated and compared with the WT protein sequence.

## Results

The WT GALT CDS was **1,140 bp** long and produced a predicted protein of **379 amino acids**. Translation began with the start codon **ATG** and ended with the stop codon **TAA** in reading frame 1. The predicted WT protein sequence matched the accepted RefSeq protein **NP_000146.2**.

For the documented mutation, nucleotide **563 changed from A to G**, changing the codon from **CAG to CGG**. Translation produced a protein of **379 amino acids**, with the amino-acid substitution **Q188R**. No frameshift, amino-acid insertion or deletion, or premature stop codon was observed.

For the artificial mutation, nucleotide **564 changed from G to A**, changing **CAG to CAA**. Both codons encode glutamine (Q). Therefore, the translated artificial mutant protein remained identical to the WT protein and was also **379 amino acids** long.

## WT versus Mutant Protein Comparison

The documented mutant protein differed from the WT protein at **amino-acid position 188**.

- **WT:** Q (glutamine) at position 188
- **Documented mutant:** R (arginine) at position 188
- **WT protein length:** 379 amino acids
- **Documented mutant protein length:** 379 amino acids
- **Frameshift:** None
- **Premature stop codon:** None
- **Amino acids inserted or deleted:** None

The sequence comparison around the affected position was:

```text
WT:     MGCSNPHPHCQVWASSFL
Mutant: MGCSNPHPHCRVWASSFL
```

Thus, the documented mutation resulted in a single amino-acid substitution without changing the overall protein length or reading frame.

## Artificial Mutation Experiment

An artificial synonymous mutation, **c.564G>A**, was introduced into a separate copy of the WT GALT CDS. This changed the codon from **CAG to CAA**. Both codons encode glutamine (Q), so the nucleotide substitution was predicted to have no effect on the amino-acid sequence.

After translation, the artificial mutant protein was identical to the WT protein and remained **379 amino acids** long. No amino-acid substitution, insertion, deletion, frameshift, or premature stop codon was observed.

This experiment demonstrates that a single-nucleotide substitution does not necessarily result in an amino-acid change because of the degeneracy of the genetic code.

## Molecular Interpretation: Gene → Mutation → Protein → Cellular Effect → Phenotype

The molecular consequence of the documented mutation can be summarized as:

**GALT gene → c.563A>G mutation → CAG to CGG codon change → p.Gln188Arg (Q188R) → altered GALT protein → reduced GALT enzymatic function → disruption of galactose metabolism → cellular and tissue effects → classic galactosemia phenotype.**

The c.563A>G substitution changes glutamine (Q) to arginine (R) at amino-acid position 188. Although the mutation does not cause a frameshift or change the protein length, the amino-acid substitution can affect the structure and function of the GALT enzyme. Published biochemical and structural studies have reported impaired GALT function associated with the Q188R variant.

Reduced GALT activity disrupts the normal Leloir pathway of galactose metabolism. This can lead to accumulation of galactose-1-phosphate and other galactose metabolites, contributing to the clinical manifestations associated with classic galactosemia.

The computational analysis demonstrates the DNA and predicted protein sequence changes, while published experimental studies provide evidence for the functional effects of the Q188R variant.

## Limitations

The experiment was based primarily on DNA sequence manipulation and computational translation using Galaxy. The analysis demonstrates the predicted effects of the nucleotide substitutions on the amino-acid sequence but does not directly measure protein expression, enzyme activity, protein stability, aggregation, or cellular effects.

The artificial c.564G>A mutation was created for educational purposes and was not intended to represent a naturally occurring disease-associated variant.

## Conclusion

The documented **GALT c.563A>G (p.Gln188Arg)** mutation produced a single amino-acid substitution from glutamine to arginine at position 188. The mutation did not change the reading frame or overall protein length.

In contrast, the artificial **c.564G>A** substitution changed the DNA sequence without changing the encoded amino acid because both CAG and CAA encode glutamine. The predicted artificial mutant protein was therefore identical to the WT protein.

Overall, the experiment demonstrates how different single-nucleotide substitutions can produce different effects on protein products and illustrates the molecular connection between a pathogenic gene mutation, altered protein function, and the phenotype associated with classic galactosemia.

## References

Berry, G. T. (2021). Classic galactosemia and clinical variant galactosemia. In *GeneReviews®*. University of Washington, Seattle.

Elsevier, J. P., & Fridovich-Keil, J. L. (1996). The Q188R mutation in human galactose-1-phosphate uridylyltransferase acts as a partial dominant negative. *Journal of Biological Chemistry, 271*(50), 32002–32007.

Fridovich-Keil, J. L., Langley, S. D., Mazur, L. A., Lennon, J. C., Dembure, P. P., & Elsas, L. J. (1995). Identification and functional analysis of three distinct mutations in the human galactose-1-phosphate uridyltransferase gene associated with galactosemia in a single family. *American Journal of Human Genetics, 56*(3), 640–646.

McCorvie, T. J., & Timson, D. J. (2011). Structural and molecular biology of type I galactosemia: Disease-associated mutations. *IUBMB Life, 63*(11), 949–954.

McCorvie, T. J., Kopec, J., Pey, A. L., Shrestha, L., Yue, W. W., & Timson, D. J. (2016). Molecular basis of classic galactosemia from the structure of human galactose 1-phosphate uridylyltransferase. *Human Molecular Genetics, 25*(11), 2234–2244.

NCBI ClinVar. GALT c.563A>G (p.Gln188Arg), Variation ID 3614.

NCBI RefSeq. *GALT* transcript NM_000155.4 and protein NP_000146.2.
