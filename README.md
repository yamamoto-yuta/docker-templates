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

Environment:
| environment | version |
| -- | -- |
| Python | 3.7.8 |

Work Dir: `/home`

Installed Commands:
- git
- vim

### jupyter-lab

#### jl-base
Simple jupyter lab image.

Environment:
| environment | version |
| -- | -- |
| Python | 3.7.8 |
| Jupyter Lab | . |

Work Dir: `/home`

Installed Commands:
- git
- vim

#### jl-extensions
Jupyter lab with extensions image.

Environment:
| environment | version |
| -- | -- |
| Python | 3.7.8 |
| Jupyter Lab | . |

Work Dir: `/home`

Installed Commands:
- git
- vim

