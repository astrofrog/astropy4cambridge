Installing Python, Astropy, and affiliated packages
===================================================

This is a quick howto for installing the required packages for the workshop.


Download and install conda
--------------------------

Download miniconda for **Linux**:

```bash
wget http://repo.continuum.io/miniconda/Miniconda-latest-Linux-x86_64.sh -O
miniconda.sh
```

Download miniconda for **MacOSX**:

```bash
wget http://repo.continuum.io/miniconda/Miniconda-3.7.3-MacOSX-x86_64.sh -O
miniconda.sh
```

```bash
bash miniconda.sh -b -p $HOME/miniconda
export PATH="$HOME/miniconda/bin:$PATH"
conda update --yes conda
conda config --add channels astropy
```

Install common Python dependencies
----------------------------------

In the workshop notebooks we have direct use of the following packages:

 - astropy
 - astroquery
 - APLpy
 - matplotlib
 - numpy
 - photutils
 - reproject
 - wcsaxes

First create and activate the environment:

```bash
conda create -n astropy_py3 python=3.5
source activate astropy_py3
```

Install all of the packages:

```bash
conda install astropy astroquery aplpy photutils wcsaxes numpy matplotlib reproject
```

