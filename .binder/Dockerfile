FROM rocker/binder:4.3.1
LABEL maintainer='Tony Stone'
COPY --chown=${NB_USER} . ${HOME}
USER ${NB_USER}



RUN wget https://github.com/UCL-CHIG/Intro2RecordLinkage/raw/master/DESCRIPTION && R -e "options(repos = list(CRAN = 'http://mran.revolutionanalytics.com/snapshot/2023-09-06/')); devtools::install_deps()"

RUN rm DESCRIPTION.1; exit 0
