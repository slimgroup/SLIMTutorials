# SLIMTutorials

This repository includes notebook tutorials in the Seismic Laboratory for Image and Modeling ([SLIM](https://slim.gatech.edu/)) group.

## TRANSFORM 22 Tutorial

[Ziyi (Francis) Yin](https://slim.gatech.edu/people/ziyi-yin) will be giving a 2-hour live talk with the title "Julia for Geoscience" at 2PM UTC on April 27 in [TRANSFORM 2022 conference](https://transform.softwareunderground.org/overview/sessions). Please visit [here](https://transform.softwareunderground.org/2022-julia-for-geoscience/) for the details and [here](https://www.youtube.com/watch?v=HyWfp3NzIbg) for the youtube link. The talk will cover a few tutorials in this repository, including:

[Introduction to Julia](https://github.com/slimgroup/SLIMTutorials/blob/main/10_intro_julia.ipynb)    
[Introduction to JOLI.jl](https://github.com/slimgroup/SLIMTutorials/blob/main/11_intro_JOLI.ipynb)    
[Introduction to JUDI.jl](https://github.com/slimgroup/SLIMTutorials/blob/main/00_intro_JUDI.ipynb)    
[SEGY File Handling in Julia with SegyIO.jl](https://github.com/slimgroup/SLIMTutorials/blob/main/01_SegyIO.ipynb)     
[Training Normalizing Flow with InvertibleNetworks.jl](https://github.com/slimgroup/SLIMTutorials/blob/main/07_normalizing_flow_training.ipynb)

Please also feel free to take a look at other notebooks in the repository if you are interested in our work. Feel free to open issue or pull request in this repository or in the software's repository.

## Running with Docker

If you don't want to manually install Julia or the Julia packages used in this repository, you can also run these tutorials on a [docker image](https://www.docker.com/). You can execute the following command in your terminal:

```bash
docker run -p 8888:8888 mloubout/judi:1.7-latest
```

This command downloads the image and launches a container. You will see a link that you can copy-paste to your browser to access the notebooks. Alternatively, you can run a bash session, in which you can start a regular interactive Julia session and run the example scripts. You can download/start the container as a bash session via the following command:

```julia
docker run -it mloubout/judi:1.7-latest /bin/bash
```

## Package availability

For any package missing in the notebooks, you can add an extra cell at the top to install the missing package:

```julia
using Pkg
Pkg.add(["Pkg1", "Pkg2", ...])
```

where `Pkg1, Pkg2, ..` are the names of the packages to be installed.

## Data

Some of the notebook require data. To download the data run
```bash
curl -L -o data.zip https://www.dropbox.com/sh/m2ksfp7wjww3jds/AADswzf_8ZdMiDW-nmrLNgJ0a
unzip data.zip -d path/to/data/you/want
```

and modify the data loading lines in the notebook according to the new path of the data folder.

## LICENSE

The software used in this repository can be modified and redistributed according to [MIT license](https://github.com/slimgroup/SLIMTutorials/blob/main/LICENSE).

## Authors

SLIM Group @ Georgia Institute of Technology, [https://slim.gatech.edu](https://slim.gatech.edu/)      
SLIM public GitHub account, [https://github.com/slimgroup](https://github.com/slimgroup).
