FROM jupyter/base-notebook

ENV TYLOR="tylor"

RUN conda install --quiet --yes \
    'numpy' \
    && \
    conda clean --al -f -y && \
    npm cache clean --force && \
    rm -rf "/home/${NB_USER}/.cache/yarn" && \
    rm -rf "/home${NB_USER}/.bode-gyp" && \
    fix-permissions "${CONDA_DIR}" && \
    fix-permissions "/home/${NB_USER}"
 
