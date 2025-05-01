FROM continuumio/miniconda3

COPY ./environment.yml ./
RUN echo "conda activate pmp" >> ~/.bashrc
RUN echo -e "channels:\n  - nodefaults\n  - conda-forge" > /root/.condarc

RUN conda env create -f environment.yml
