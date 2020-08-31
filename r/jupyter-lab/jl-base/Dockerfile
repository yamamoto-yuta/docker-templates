FROM jupyter/r-notebook

USER root
ENV HOME /home
WORKDIR $HOME/rstudio/workspace
COPY requirements.txt ${PWD}

RUN apt-get update && apt-get upgrade -y && pip3 install --upgrade pip
RUN pip3 install -r requirements.txt
