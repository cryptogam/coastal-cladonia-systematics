# coastal-cladonia-systematics

This repo holds the sequencing data and analysis for the coastal *Cladonia* systematics project led by Bri Baumbach and Niko Darci-Maher :)

## lab work prelude

In short, we collected *Cladonia* lichens in the field, extracted DNA, amplified the ITS region by PCR, and ran Sanger sequencing.

## assemble ITS reads 

Use Geneious to assemble individual ITS reads, and export them as .fasta files.

## run multiple sequence alignment
Merge fasta files into a single input file
```
cd data
cat *.fasta > 2025_cladonia_ITS_all.fasta
cd ..
```

Use MAFFT to align these ITS sequences
```
mafft data/2025_cladonia_ITS_all.fasta > mafft_cladonia_all
```
