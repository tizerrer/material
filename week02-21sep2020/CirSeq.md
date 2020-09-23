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

## Application

Determination of virus mutation rates is difficult and often unreliable because accuracy depends on observing rare events, but the accuracy improvement of CirSeq compared to conventional next-generation sequencing allows the capture of a near-complete distribution of mutant frequencies within RNA virus populations. Also, CirSeq allows for a better transition-to-transversion ratio (ts:tv). These nucleotide-specific differences in mutation rate likely reflect the molecular mechanism of viral polymerase fidelity, which can help understanding the directionality of evolution.

Source: [1, Main].

## Statistics

TODO

## References

[1] 
Ashley Acevedo, Leonid Brodsky & Raul Andino.
Mutational and fitness landscapes of an RNA virus revealed through population sequencing. 
[Nature 505, pp. 686-690 (2014)](https://www.nature.com/articles/nature12861).

## Authors of this document

[numpde](https://github.com/numpde/) (RA)
[johaab](https://github.com/johaab/) (JH)
...
