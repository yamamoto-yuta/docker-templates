FROM ubuntu:20.04

ENV HOME /home
WORKDIR $HOME/
COPY .bashrc .vimrc $HOME/

RUN apt-get update && apt-get upgrade -y \
  && apt-get install -y \
    git \
    vim

