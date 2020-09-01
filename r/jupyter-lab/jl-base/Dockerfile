FROM jupyter/r-notebook

USER root
ENV HOME /home
WORKDIR $HOME/
COPY requirements.txt $HOME/

RUN apt-get update && apt-get upgrade -y && pip3 install --upgrade pip
RUN pip3 install -r $HOME/requirements.txt

