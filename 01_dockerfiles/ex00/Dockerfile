FROM alpine

LABEL vendor1="Ecole 42 - Docker-1"
LABEL com.example.release-date="2019-02-28"
MAINTAINER tavelino <tavelino@student.42.fr>

RUN apk update && \
apk upgrade && \
apk add vim 

ENTRYPOINT vim

## Usage:
## 1 build 
# docker build -t ex00
## 2 then run
# docker run --rm -ti ex00
##  source: https://docs.docker.com/engine/reference/builder/
##
## FROM: Informa a partir de qual imagem será gerada a nova imagem, lembrando que em poucos casos (Veremos em posts futuros), uma imagem será gerada se um imagem base;
## LABEL: Adiciona metadados a uma imagem, informações adicionais que servirão para identificar versão, tipo de licença, ou host, lembrando que a cada nova instrução LABEL é criada uma nova layer, o Docker recomenda que você não use muitas LABEL. É possível realizar filtragens posteriormente utilizando essas LABEL.
## MAINTAINER: Campo opcional, que informa o nome do mantenedor da nova imagem;
## RUN: Especifica que o argumento seguinte será executado, ou seja, realiza a execução de um comando;
## ENTRYPOINT: Informa qual comando será executado quando um container for iniciado utilizando esta imagem, diferentemente do 
## source: https://www.mundodocker.com.br/o-que-e-dockerfile/
