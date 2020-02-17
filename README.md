## CFIA Conda Recipes

Repository of conda recipes

### Requirements

- conda
- conda-build
- anaconda

If you need to install conda:

```
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh -O miniconda.sh;
bash miniconda.sh -b -p $HOME/miniconda
conda update -q conda
```

Install the required packages
```
conda install -y anaconda-client conda-build
```

### Usage

From within the repo:
```
conda build repo_name
anaconda upload -u olcbioinformatics /path/to/repo_name-version_info.tar.bz2
```
