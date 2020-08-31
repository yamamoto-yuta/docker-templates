FROM jupyter/r-notebook

USER root
ENV HOME /home
WORKDIR $HOME/rstudio/workspace
COPY requirements.txt $HOME/

RUN apt-get update && apt-get upgrade -y

