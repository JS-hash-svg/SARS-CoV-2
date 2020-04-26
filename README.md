# SARS-CoV-2 data sets visualized by `dms-view`

## Data sets

### Spike

* [./data/BloomLab2020](data/BloomLab2020) maps natural variation among SARS-like coronavirus isolates from human, bat, and other host species onto Spike trimer and ACE2-bound RBD structures. Links to `dms-view` for [Spike]() and [RBD]() visualizations.

## Adding data sets

1. Make a new branch or a fork of this repository.

2. Navigate to the [./data/](data) directory and create a subdirectory for the appropriate protein and study.
   Data are organized first by protein and then by study, with studies named by the first author and year, such as [./data/Spike/BloomLab2020/](data/Spike/BloomLab2020).

3. Within that subdirectory, add the three input files that are needed to visualize the data.
   As described in the [`dms-view` docs](https://dms-view.github.io/docs/), these are a CSV file of the data, a protein structure PDB file, and a Markdown metadata file.
   In general, you should name these with the CSV data file named according to the study name (e.g., [./data/Spike/BloomLab2020/BloomLab2020.csv](data/Spike/BloomLab2020/BloomLab2020.csv)), the PDB file simply being the PDB (e.g., [./data/Spike/BloomLab2020/6vyb.pdb](./data/Spike/BloomLab2020/6vyb.pdb)), and the Markdown metadata file also named according to the study name (e.g. [./data/Spike/BloomLab2020/BloomLab2020.md](data/Spike/BloomLab2020/BloomLab2020.md)).
   In addition, you should add a README within the subdirectory explaining the origin of the files (e.g., [./data/Spike/BloomLab2020/README.md](data/Spike/BloomLab2020/README.md)).
   In some cases (such as if the same data is mapped to multiple protein structures) you may need to extend or modify this naming scheme.
   If you need to process other rawer forms of the data (e.g., from paper supplements) into the final data file for `dms-view`, then include those rawer data and the processing scripts if possible, explaining in the subdirectory repo.

4. Make a pull request for your branch or fork to add the data.

5. In [this top-level README file](README.md) add a **short** description of the study and a link to an appropriate [dms-view](https://dms-view.github.io) view of the dataset.

6. Make a pull request for your branch or fork to add the link.
