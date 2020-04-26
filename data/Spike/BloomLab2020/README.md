# natural amino-acid frequencies in Spike

Tyler curate an [alignment](Spikes.fasta) based on the sequences in the Extended Data Fig 1 of [Letko, Marzi, and Munster (2020)](https://www.nature.com/articles/s41564-020-0688-y) and the two pangolin sequences from [Lam _et al._ (2020)](https://www.nature.com/articles/s41586-020-2169-0).

We are using the pdb structure [6vyb.pdb](https://www.rcsb.org/structure/6VYB)

The [Snakefile](Snakefile) reads in the protein sequences and the protein structure and generates the datafile [results/Letko_spike.csv](results/Letko_spike.csv).
To run the snakemake pipeline, you can use the conda environment `Letko2020`.
To build the environment run `conda env create -f env.yml`.
