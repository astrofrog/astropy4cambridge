Installing Python, Astropy, and affiliated packages
===================================================

This is a quick howto for installing the required packages for the workshop.


Download and install conda
--------------------------

Download miniconda for **Linux**::

    wget http://repo.continuum.io/miniconda/Miniconda-latest-Linux-x86_64.sh -O miniconda.sh


Download miniconda for **MacOSX**::

    wget http://repo.continuum.io/miniconda/Miniconda-latest-MacOSX-x86_64.sh -O miniconda.sh


Set up conda::

    bash miniconda.sh -b -p $HOME/miniconda
    export PATH="$HOME/miniconda/bin:$PATH"
    conda update --yes conda
    conda config --add channels astropy


Install common Python dependencies
----------------------------------

In the workshop notebooks we have direct use of the following packages. Some
of them have optional dependencies we will use indirectly (e.g. scipy,
scikit-image):

 - astropy
 - astroquery
 - APLpy
 - matplotlib
 - numpy
 - photutils
 - reproject
 - wcsaxes


Install all of the packages (including their dependencies)::

    conda install jupyter astropy astroquery aplpy photutils wcsaxes numpy matplotlib reproject scipy scikit-image


