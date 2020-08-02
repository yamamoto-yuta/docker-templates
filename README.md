# docker-templates
Templates for Docker

# Usage
Build image from docker-compose.
```
$ docker-compose up -d --build
$ docker exec -it <CONTAINER_ID> bash
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
- Jupyter Lab

JupyterLab-Extensions:
- @jupyter-widgets/jupyterlab-manager

@jupyter-widgets/jupyterlab-manager

Work Dir: `/home`

Installed Commands:
- git
- vim

