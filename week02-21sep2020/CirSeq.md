# Circular sequencing (CirSeq) of viral RNA

DRAFT

## What it does

Circularized genomic RNA fragments are used to generate tandem repeats.
They then serve as substrates for next-generation sequencing.
This provides sequence redundancy for each genomic fragment derived from a single individual within the virus population.
Observed differences in each redundant set must originate from enzymatic or sequencing errors and can be filtered statistically.
This overcomes the limitations of next-generation sequencing error. 

Source: [1, Main].

## Technology

Viral population is multiplied in vivo. 
RNA extracted from the viral population is purified, fragmented, size-selected, circularized, reverse-transcribed,
and cloned. 
These libraries are sequences on Illumina (MiSeq).
Bowtie 2 and custom analysis software are used for sequence mapping,
identifying and aligning repeats.
A majority-vote consensus is established between redundant reads
and 
error probabilities are estimated.

Source: [1, Methods].

## References

[1] 
Ashley Acevedo, Leonid Brodsky & Raul Andino.
Mutational and fitness landscapes of an RNA virus revealed through population sequencing. 
[Nature 505, pp. 686-690 (2014)](https://www.nature.com/articles/nature12861).

## Authors of this document

[numpde](https://github.com/numpde/) (RA)
...
