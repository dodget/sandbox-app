FROM jupyter/base-notebook

RUN conda install --quiet --yes \
    'numpy' \
    'pandas' \
    && \
    conda clean --al -f -y && \
    npm cache clean --force && \
    rm -rf "/home/${NB_USER}/.cache/yarn" && \
    rm -rf "/home${NB_USER}/.bode-gyp" && \
    fix-permissions "${CONDA_DIR}" && \
    fix-permissions "/home/${NB_USER}"
 
