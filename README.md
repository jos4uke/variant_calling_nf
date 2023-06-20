# VITI-CALL NextFlow pipeline
> **An open-source analysis pipeline to detect variants from whole genome or targeted sequencing**

## Introduction

**VITI-CALL** Nextflow pipeline is a workflow designed to detect variants on whole genome or targeted sequencing data, designed to work on Vitis genome. 
The pipeline is built using [Nextflow](https://www.nextflow.io), a workflow tool to run tasks across multiple compute infrastructures in a very portable manner. It uses Docker/Singularity containers making installation trivial and results highly reproducible.
It was initially developped on snakemake workflow engine for the Vitis 4k project (Sophie Blanc, Camille Rustenholz et al., INRAE, 2020-2023). it is a complete rewrite using [Nextflow DSL2](https://www.nextflow.io/docs/latest/dsl2.html) of this pipeline, using one container per process which makes it easier to maintain and update dependencies. 

todo: add a workflow image

## From workflow template 

Give a general description of the workflow, the instructions on how to run it, how to build the docker images starting from Dockerfiles (if necessary), what are the parameters (meaning, permitted values, etc.) and the expected output.

* *main.nf* file should contains the main Nexflow workflow
* *modules* directory should contains all the Nextflow files (one per module / process)
* *nextflow.config* file should contains all the directives about which docker image to use per module / process as well as number of CPUs and RAM
* *dockerfiles* directory should contains all the Dockerfile needed to build Docker images in case the image is not already present and downloadable from BIOCONDA (https://bioconda.github.io/) or DockerHUB (https://hub.docker.com/)
