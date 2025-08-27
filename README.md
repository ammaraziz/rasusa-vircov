# wastewater subsampling pipeline

[![DOI](https://zenodo.org/badge/988197048.svg)](https://doi.org/10.5281/zenodo.16956130)

### How to run

Git clone this repo and run snakemake:

```
snakemake -j 10 --use-conda
```

### outputs:

1. Subsampled reads to specified amount in `results/subsampled
2. vircov output in `results/vircov`
3. concatenated vircov results in`results/vircov/all.combined.tsv`
4. plots in `scripts`, R script must be run manually.

### Plots

1. `rc` references to `remap consensus` value in the vircov output
2. `cc` references to `consensus consensus` value in the vircov output
3. For `rc` and `cc` plots, the flu segments 4,5,6 (HA,NA,MP) were used instead of the full genome. Values were averaged.
4. The `*_flu` plot contains segments variability.

