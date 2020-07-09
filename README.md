# SARS-CoV-2 data sets visualized by `dms-view`

## Data sets

### Spike

* [./data/Spike/BloomLab2020](data/Spike/BloomLab2020) maps natural variation among SARS-like coronavirus isolates from human, bat, and other host species onto Spike trimer and ACE2-bound RBD structures. Links to `dms-view` for [Spike](https://dms-view.github.io/?pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FSARS-CoV-2%2Fmaster%2Fdata%2FSpike%2FBloomLab2020%2F6vyb.pdb&markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FSARS-CoV-2%2Fmaster%2Fdata%2FSpike%2FBloomLab2020%2FBloomLab_spike.md&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FSARS-CoV-2%2Fmaster%2Fdata%2FSpike%2FBloomLab2020%2Fresults%2FBloomLab2020_spike.csv&condition=natural+frequencies&site_metric=site_entropy&mutation_metric=mut_frequency&selected_sites=) and [RBD](https://dms-view.github.io/?pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FSARS-CoV-2%2Fmaster%2Fdata%2FSpike%2FBloomLab2020%2F6m0j.pdb&markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FSARS-CoV-2%2Fmaster%2Fdata%2FSpike%2FBloomLab2020%2FBloomLab_rbd.md&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2FSARS-CoV-2%2Fmaster%2Fdata%2FSpike%2FBloomLab2020%2Fresults%2FBloomLab2020_rbd.csv&condition=natural+frequencies&site_metric=site_entropy&mutation_metric=mut_frequency&selected_sites=) visualizations.
* Mutational effects on binding and expression as measured by [Starr, Greaney, _et al.,_ 2020](https://www.biorxiv.org/content/10.1101/2020.06.17.157982v1). Click [here](https://dms-view.github.io/?markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fjbloomlab%2FSARS-CoV-2-RBD_DMS%2Fmaster%2Fresults%2Fdms_view%2Fdescription_RBD.md&pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fjbloomlab%2FSARS-CoV-2-RBD_DMS%2Fmaster%2Fdata%2Fstructures%2FACE2-bound%2F6m0j.pdb&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fjbloomlab%2FSARS-CoV-2-RBD_DMS%2Fmaster%2Fresults%2Fdms_view%2Fdms-view_table_RBD.csv&condition=ACE2-binding&site_metric=site_entropy&mutation_metric=mut_preference&selected_sites=498%2C501) to see the effects mapped onto the ACE2-bound RBD structure and [here](https://dms-view.github.io/?markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fjbloomlab%2FSARS-CoV-2-RBD_DMS%2Fmaster%2Fresults%2Fdms_view%2Fdescription_spike.md&pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fjbloomlab%2FSARS-CoV-2-RBD_DMS%2Fmaster%2Fdata%2Fstructures%2FACE2-bound%2F6vxx.pdb&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fjbloomlab%2FSARS-CoV-2-RBD_DMS%2Fmaster%2Fresults%2Fdms_view%2Fdms-view_table_spike.csv&condition=ACE2-binding&site_metric=site_entropy&mutation_metric=mut_preference&selected_sites=498%2C501) to see the effects mapped onto Spike Trimer. The raw data are [here](https://github.com/jbloomlab/SARS-CoV-2-RBD_DMS).

## Adding data sets

1. Make a new branch or a fork of this repository.

2. Navigate to the [./data/](data) directory and create a subdirectory for the appropriate protein and study.
   Data are organized first by protein and then by study, with studies named by the first author and year, such as [./data/Spike/BloomLab2020/](data/Spike/BloomLab2020).

3. Within that subdirectory, add the three input files that are needed to visualize the data.
   As described in the [`dms-view` docs](https://dms-view.github.io/docs/), these are a CSV file of the data, a protein structure PDB file, and a Markdown metadata file.
   In general, you should name these with the CSV data file named according to the study name (e.g., [./data/Spike/BloomLab2020/results/BloomLab2020_spike.csv](data/Spike/BloomLab2020/results/BloomLab2020_spike.csv)), the PDB file simply being the PDB (e.g., [./data/Spike/BloomLab2020/6vyb.pdb](./data/Spike/BloomLab2020/6vyb.pdb)), and the Markdown metadata file also named according to the study name (e.g. [./data/Spike/BloomLab2020/BloomLab2020_spike.md](data/Spike/BloomLab2020/BloomLab2020_spike.md)).
   In addition, you should add a README within the subdirectory explaining the origin of the files (e.g., [./data/Spike/BloomLab2020/README.md](data/Spike/BloomLab2020/README.md)).
   In some cases (such as if the same data is mapped to multiple protein structures) you may need to extend or modify this naming scheme.
   If you need to process other rawer forms of the data (e.g., from paper supplements) into the final data file for `dms-view`, then include those rawer data and the processing scripts if possible, explaining in the subdirectory repo.

4. Make a pull request for your branch or fork to add the data.

5. In [this top-level README file](README.md) add a **short** description of the study and a link to an appropriate [dms-view](https://dms-view.github.io) view of the dataset.

6. Make a pull request for your branch or fork to add the link.
