<img width="200" alt="FUGUE Logo" src="https://github.com/user-attachments/assets/20de3361-74e5-472a-a897-141653b8a342">

# Introduction
FUGUE (_<ins>F</ins>ungal <ins>U</ins>niverse <ins>G</ins>enome <ins>U</ins>nification <ins>E</ins>ngine_) is a Python tool that allows you to download genomes, CDS, GFF, and proteomes for more than 2,000 fungal species used in its parent project, [ALLEGRO](https://github.com/ucrbioinfo/allegro). It draws data from [NCBI Datasets](https://www.ncbi.nlm.nih.gov/datasets/), [FungiDB](https://fungidb.org/), [EnsemblFungi](https://fungi.ensembl.org/index.html), and [MycoCosm](https://mycocosm.jgi.doe.gov/mycocosm/home), and removes duplicate downloads. Additionally, FUGUE can:

1. Create CDS from downloaded GFF files and mark the intron/exon boundaries using [GFFRead](https://github.com/gpertea/gffread)
1. Utilize [DIAMOND](https://github.com/bbuchfink/diamond) to create orthogroups for your genes of interest
1. Create the required input for ALLEGRO

Note that you do NOT need to use FUGUE to replicate the results shown in the ALLEGRO publication. All data used in our experiments are provided on the ALLEGRO repository and on Zenodo. This repository shows you how we did it, but we provide you with the data we used.

# Documentation
You may find the documentation for FUGUE at its [GitHub Wiki](https://github.com/ucrbioinfo/fugue/wiki).

# Support
If you run into any issues or have any suggestions for FUGUE, please report them on our GitHub Issues tracker. It's the fastest way to get support and helps us improve FUGUE for everyone. You may also email the authors at their provided e-mail addresses on the publication directly.

# About
FUGUE has been developed and is maintained by <ins>Amir</ins>sadra Mohseni, and Stefano Lonardi at the University of California, Riverside.

# Disclaimer
For programmers, if you open one of the scripts and see hard-coded paths, do not panic (e.g., [this line](https://github.com/ucrbioinfo/fugue/blob/a2af815aa387e9682d4c5ef2621eadd89f68f05e/src/utils/diamond/5_run_bidirectional_diamond.sh#L5)). Following the Wiki instructions, you will set your own paths and these scripts will be updated accordingly.
