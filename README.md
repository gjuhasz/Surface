This is a project to 


## Installation 

### Main packages

- ase: a general framework to represent chemical structures and run the calculations
- DFTB+: the DFTB calculator



### Environment


```
conda create --name old_ase+dftb+ mlenv python==3.10 pandas numpy=1.22.1

conda activate old_ase+dftb+ 
conda install ase
conda install spglib psycopg2 pyamg pytest

conda config --add channels conda-forge
conda install -n base mamba
    or 
conda install mamba -yc conda-forge

mamba install 'dftbplus=*=mpi_openmpi_*'
mamba install dftbplus-tools dftbplus-python
```

check ase:
```

```



**Note:** there is a compartibility issue between latest DFTB+ and ase, that is why using the strange versions

**Error Note:** if mamba installation is difficult (*mamba gives error messages, most probably mixing up default and conda-forge chanells*) try `conda install mamba -yc conda-forge` instead of installing in base 