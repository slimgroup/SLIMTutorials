# ML4SeismicTutorials

Tutorials for the 2021 ML4Seismic Partners Meeting


## Guidelines

This series of tutorials is meant to show simple examples of how to use our software. If you are un-familiar with julia and notebooks in general, let us know and we will have a walk-through of the basics.

## Package availability

For simplicity, only the most basic packages are installed in the environment. For any package missing in the notebooks, you can add an extra cell at the top to install the missing package:

```julia
using Pkg
Pkg.add(["Pkg1", "Pkg2", ...])
```

where `Pkg1, Pkg2, ..` are the names of the packages to be installed. These packages will be installed in your user environment and will not impact other users.

## Data

Some of the notebook require data. On the jupyterhub we setup, the data is pre-downloaded in the path used in the notebooks but you will it to download it yourself to run the tutorials on your own machine. To download the data run
```bash
curl -L -o data.zip https://www.dropbox.com/sh/m2ksfp7wjww3jds/AADswzf_8ZdMiDW-nmrLNgJ0a?dl=0
unzip data.zip -d path/to/data/you/want
```

and modify the data loading lines in the notebook according to the new path of the data folder.
