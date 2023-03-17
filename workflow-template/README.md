# Workflow template title
Give a general description of the workflow, the instructions on how to run it, how to build the docker images starting from Dockerfiles (if necessary), what are the parameters (meaning, permitted values, etc.) and the expected output.

* *main.nf* file should contains the main Nexflow workflow
* *modules* directory should contains all the Nextflow files (one per module / process)
* *nextflow.config* file should contains all the directives about which docker image to use per module / process as well as number of CPUs and RAM
* *dockerfiles* directory should contains all the Dockerfile needed to build Docker images in case the image is not already present and downloadable from BIOCONDA (https://bioconda.github.io/) or DockerHUB (https://hub.docker.com/)