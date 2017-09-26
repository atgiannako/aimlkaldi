FROM georgepar/kaldi
MAINTAINER Athanasios Giannakopoulos

RUN apt-get -y install vim curl gawk

WORKDIR /kaldi/tools
RUN curl -LJO https://github.com/atgiannako/aimlkaldi/raw/master/srilm.tgz
RUN bash -c ./install_srilm.sh

RUN mkdir -p /kaldi/egs/aiml-asr

WORKDIR /

ENTRYPOINT ["/bin/bash"]
