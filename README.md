# Metropolis algorithm
<p align="center">
  <img src="met3d_w_git.gif" />
</p>

# Topological Data Analysis
<p align="center">
  <img src="ducks.gif" />
</p>

# Python workflow "cheatsheet"
- delete last git stash: `git stash drop`
- remove old jupyter kernels: `jupyter kernelspec uninstall unwanted-kernel`
- pull all data from all submodules: `git submodule update --init --recursive`
- remove a conda environment completely: `conda remove --name myenv --all`
- new submodule: `git submodule add <https_url>`
- update all submodules: `git submodule update --remote --merge`, then commit the new gitlink
- list all jupyter kernels: `jupyter kernelspec list`
- install a new jupyter kernel for a python interpreter in a conda env `python -m ipykernel install --user --name=<CONDA ENV NAME> --display-name="$(python --version): <PRETTY NAME>"`
