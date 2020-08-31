# docker-templates

Templates for Docker

# Usage

## Download

Download templates by using 'svn'.
```
$ svn export https://github.com/yamamoto-yuta/docker-templates/trunk/<DIRECTORY_PATH>
```

The way to use container is different for each templates.

# Templates

## Python

### Usage

```
$ docker-compose up -d --build
$ docker exec -it <CONTAINER_ID> bash
```

### Image list

| Image name | Python Ver. | Work Dir. | Commands | Libraries | Extensions |
|---|---|---|---|---|---|
| base | 3.7.8 | `/home` | git , vim |  |  |
| jupyter-lab/jl-base | 3.7.8 | `/home` | git , vim | jupyterlab |  |
| jupyter-lab/jl-extensions | 3.7.8 | `/home` | git , vim | jupyterlab |  |
| jupyter-lab/jl-custom | 3.7.8 | `/home` | git , vim | jupyterlab <br> numpy <br> pandas <br> tqdm | @jupyter-widgets/jupyterlab-manager <br> @lckr/jupyterlab_variableinspector <br> @jupyterlab/toc |

---

## R

### Usage

#### R Studio

1. Build & up
```
$ docker-compose up -d --build
```

2. Access to `https:localhost:<PORT_NUM(8787)>`
3. Input username(`rstudio`) and password(`pass`)

#### Jupyter Lab

```
$ docker-compose up -d --build
$ docker-compose run <CONTAINER_NAME>
```

### Image list

| Image name | Work Dir. | Packages |
|---|---|---|
| r-studio/rs-base | `/home/rstudio/workspace` |  |
| r-studio/rs-ts | `/home/rstudio/workspace` | xts <br> forecast <br> urca <br> tseries <br> ggplot2 <br> ggfortify |
| jupyter-lab/jl-base | `/home/rstudio/workspace` |  |
| jupyter-lab/jl-ts | `/home/rstudio/workspace` | xts <br> forecast <br> urca <br> tseries <br> ggplot2 <br> ggfortify |

---

## Ubuntu

### Usage

```
$ docker exec -it <CONTAINER_ID> bash
```

### Image list

| Image name | Ubuntu Ver. | Work Dir. | Commands |
| -- | -- | -- | -- |
| ubuntu/base | 20.04 | `/home` | git, vim
