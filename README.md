# docker-templates
Templates for Docker

# Usage

## Download

Download templates by using 'svn'.
```
$ svn export https://github.com/yamamoto-yuta/docker-templates/trunk/<DIRECTORY_PATH>
```

## Build

Build image from docker-compose.
```
$ docker-compose up -d --build
```

The way to use container is different for each templates.

# Templates

## Python
Usage:
```
$ docker exec -it <CONTAINER_ID> bash
```

Image list:
| Image name | Python Ver. | Work Dir. | Commands | Libraries | Extensions |
| -- | -- | -- | -- | -- | -- |
| python/base | 3.7.8 | `/home` | git <br> vim | | |
| jupyter-lab/jl-base | 3.7.8 | `/home` | git <br> vim | jupyterlab | |
| jupyter-lab/jl-extensions | 3.7.8 | `/home` | git <br> vim | jupyterlab | |
| jupyter-lab/jl-custom | 3.7.8 | `/home` | git <br> vim | jupyterlab <br> numpy <br> pandas <br> tqdm | @jupyter-widgets/jupyterlab-manager <br> @lckr/jupyterlab_variableinspector <br> @jupyterlab/toc |

## R
Usage:
1. Access to `https:localhost:<PORT_NUM(8787)>`
2. Input username(`rstudio`) and password(`pass`)

Image list:
| Image name | Work Dir. | Packages |
| -- | -- | -- |
| r/base | `/home/rstudio/workspace` | |
| r/ts | `/home/rstudio/workspace` | xts <br> forecast <br> urca <br> tseries <br> ggplot2 <br> ggfortify |

## Ubuntu
Usage:
```
$ docker exec -it <CONTAINER_ID> bash
```

Image list:
| Image name | Ubuntu Ver. | Work Dir. | Installed Commands |
| -- | -- | -- | -- |
| ubuntu/base | 20.04 | `/home` | git, vim
