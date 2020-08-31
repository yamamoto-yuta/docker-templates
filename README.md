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

| Image name                  | Python Ver\. | Work Dir\. | Commands     | Libraries                                   | Extensions                                                                                          |
|-----------------------------|--------------|------------|--------------|---------------------------------------------|-----------------------------------------------------------------------------------------------------|
| python/base                 | 3\.7\.8      | `/home`   | git <br> vim |                                             |                                                                                                     |
| jupyter\-lab/jl\-base       | 3\.7\.8      | `/home`   | git <br> vim | jupyterlab                                  |                                                                                                     |
| jupyter\-lab/jl\-extensions | 3\.7\.8      | `/home`   | git <br> vim | jupyterlab                                  |                                                                                                     |
| jupyter\-lab/jl\-custom     | 3\.7\.8      | `/home`   | git <br> vim | jupyterlab <br> numpy <br> pandas <br> tqdm | @jupyter\-widgets/jupyterlab\-manager <br> @lckr/jupyterlab\_variableinspector <br> @jupyterlab/toc |
|                             |              |            |              |                                             |                                                                                                     |

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
$ docker-compose build
$ docker-compose run <CONTAINER_NAME>
```

### Image list

| Image name        | Work Dir\.                 | Packages                                         |
|-------------------|----------------------------|--------------------------------------------------|
| r\-studio/base    | \`/home/rstudio/workspace` |                                                  |
| r\-studio/ts      | \`/home/rstudio/workspace` | forecast, ggfortify, ggplot2, tseries, urca, xts |
| jupyter\-lab/base | \`/home/rstudio/workspace` |                                                  |

---

## Ubuntu

### Usage

```
$ docker exec -it <CONTAINER_ID> bash
```

### Image list

| Image name | Ubuntu Ver. | Work Dir. | Installed Commands |
| -- | -- | -- | -- |
| ubuntu/base | 20.04 | `/home` | git, vim
