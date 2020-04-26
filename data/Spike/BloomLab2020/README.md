# Natural amino-acid frequencies in Spike

The [raw sequences](Spikes.fasta) contains Spike amino acid sequences from various SARS-related coronaviruses. This fasta file gives the common name and accession number (NCBI or GISAID) for each isolate's genome. The current sequence set includes:
* The curated set of 30 sequences from [Letko, Marzi, and Munster (2020)](https://www.nature.com/articles/s41564-020-0688-y), which contained all known unique RBD sequences at the time of its publication. See [Extended Data Fig 1](https://www.nature.com/articles/s41564-020-0688-y/figures/6) for more information.
* RaTG13 and RmYN02, two newly described bat CoV sequences that are the most closely related strains currently known to SARS-CoV-2.
* Two recent pangolin CoV sequences from [Lam _et al._ (2020)](https://www.nature.com/articles/s41586-020-2169-0), including the infectious virus isolated from a pangolin seized in Guanxi, and the consensus sequence from two closely related isolates from pangolins seized in Guangdong.

We are using the pdb structures [6vyb.pdb](https://www.rcsb.org/structure/6VYB) for full trimer, and [6m0j.pdb](https://www.rcsb.org/structure/6M0J) for ACE2-bound RBD.

The [Snakefile](Snakefile) reads in the protein sequences and the protein structure and generates the datafiles [results/BloomLab_spike.csv](results/BloomLab_spike.csv) and [results/BloomLab_rbd.csv](results/BloomLab_rbd.csv), along with alignments which are saved in [./results](results).
To run the snakemake pipeline, you can use the conda environment `SpikeVariation`.
To build the environment run `conda env create -f env.yml`.
