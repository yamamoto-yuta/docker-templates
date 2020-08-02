# docker-templates
Templates for Docker

# Usage

## Build

Build image from docker-compose.
```
$ docker-compose up -d --build
$ docker exec -it <CONTAINER_ID> bash
```

## Download
Download templates by using 'svn'.
```
$ svn export https://github.com/yamamoto-yuta/docker-templates/trunk/<DIRECTORY_PATH>
```

# Templates

## python

### base
Simple python images

Python Version: 3.7.8

Work Dir: `/home`

Installed Commands:
- git
- vim

### jupyter-lab

#### jl-base
Simple jupyter lab image.

Python Version: 3.7.8

Libraries:
- jupyterlab

Work Dir: `/home`

Installed Commands:
- git
- vim

#### jl-extensions
Jupyter lab with extensions image.

Python Version: 3.7.8

Libraries:
- jupyterlab

JupyterLab-Extensions:
- @jupyter-widgets/jupyterlab-manager

Work Dir: `/home`

Installed Commands:
- git
- vim


#### jl-custom
Customized Jupyter lab with extensions image.

Python Version: 3.7.8

Libraries:
- jupyterlab
- numpy
- pandas
- tqdm

JupyterLab-Extensions:
- @jupyter-widgets/jupyterlab-manager
- @lckr/jupyterlab_variableinspector
- @jupyterlab/toc

Work Dir: `/home`

Installed Commands:
- git
- vim

