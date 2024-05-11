![Rhombus TDA](rhombus.gif)

# Python workflow "cheatsheet"
- delete last git stash: `git stash drop`
- remove old jupyter kernels: `jupyter kernelspec uninstall unwanted-kernel`
- pull all data from all submodules: `git submodule update --init --recursive`
- remove a conda environment completely: `conda remove --name myenv --all`
- new submodule: `git submodule add <https_url>`
- update all submodules: `git submodule update --remote --merge`, then commit the new gitlink
- list all jupyter kernels: `jupyter kernelspec list`
- install a new jupyter kernel for a python interpreter in a conda env `python -m ipykernel install --user --name=<CONDA ENV NAME> --display-name="$(python --version): <PRETTY NAME>"`

A jupyter kernel is basically something which allows you to access other conda environments using the same jupyter notebook server.

# The best makefile to ever exist on a Linux computer
```
USER=your user name goes here
HOME=/home/$(USER)

all: update clean
	ldconfig && updatedb
	screenfetch

update:
	apt-get install -f
	apt-get update
	apt-get upgrade -y

clean:
	apt autoclean
	apt autoremove -y

   
.PHONY: all update clean
```
