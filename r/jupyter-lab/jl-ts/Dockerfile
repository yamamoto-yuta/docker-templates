FROM jupyter/r-notebook

USER root
ENV HOME /home
WORKDIR $HOME/
COPY requirements.txt $HOME/

RUN apt-get update && apt-get upgrade -y && pip3 install --upgrade pip
RUN pip3 install -r $HOME/requirements.txt

# 高機能な時系列データの型を提供するパッケージ
RUN R -e "install.packages('xts', dependencies = TRUE, repos='http://cran.rstudio.com/')"
# 時系列モデルの作成と予測のためのパッケージ
RUN R -e "install.packages('forecast', dependencies = TRUE, repos='http://cran.rstudio.com/')"
# 単位根検定などを行うためのパッケージ
RUN R -e "install.packages('urca', dependencies = TRUE, repos='http://cran.rstudio.com/')"
# 残差の正規性の検定などを行うためのパッケージ
RUN R -e "install.packages('tseries', dependencies = TRUE, repos='http://cran.rstudio.com/')"
# 美麗なグラフを描くためのパッケージ
RUN R -e "install.packages('ggplot2', dependencies = TRUE, repos='http://cran.rstudio.com/')"
RUN R -e "install.packages('ggfortify', dependencies = TRUE, repos='http://cran.rstudio.com/')"

