```python
# create & activate
conda create -n proj python=3.11
conda activate proj

# install
conda install pandas numpy matplotlib scikit-learn jupyterlab
# or
mamba install ...

# search packages
conda search lightgbm

# list packages
conda list

# export env (from what you asked for, not every sub-dependency)
conda env export --from-history > environment.yml

# update conda/mamba
conda update -n base conda
mamba self-update   # if using mamba

# clean caches to fix clutter or solver slowness
conda clean -a

# remove an env you broke
conda env remove -n proj
```