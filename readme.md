# A template for experiments workspace
![](https://img.shields.io/badge/current_version-v0.1.1-blue)
![](https://github.com/stracquadaniolab/cookiecutter-workspace-nf/workflows/build/badge.svg)

A directory structure to build a workspace for experiments.

## Directory structure

```
.
|-- conf
|-- data
|-- resources
|-- logs
|-- readme.md
`-- results
```

The `conf` directory contains Nextflow config files to run a pipeline; you must
define the parameters of each experiment in a config file rather than passing
them on the command line for reproducibility.

The `data` directory contains data to be processed by a pipeline. This directory
usually contains the raw data (e.g. data from sequencing experiments). You
should take some time to organise it in a meaningful and consistent way.

The `resources` directory contains data retrieved from external sources, like
annotation files (e.g. genome GFF) or geneset GMT files.

The `logs` directory contains the log of each pipeline run.

The `results` directory contains the result of experiments. You should take some
time to organise it in a meaningful and consistent way.

The readme.md file contains a description of the project and how the data and
results folder are organised.

## Authors

* Giovanni Stracquadanio, giovanni.stracquadanio@ed.ac.uk
