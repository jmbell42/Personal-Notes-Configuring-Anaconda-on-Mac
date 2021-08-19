# Personal-Notes-Configuring-Anaconda-on-Mac


Note: When configuring GITM Python Codes on a Mac, several packages are needed.  Some are easy:

1. Spacepy
2. SolarPy

Some are a pain:

1.  Cartopy:  Need to use a specific algorithm in Conda to get Cartopy to install.  Cartopy is housed on conda forge

  You should be able to simply run:    >>  conda install -c conda-forge cartopy
  Note:  You can add conda-forge to your default path with:
            >> conda config --add channels conda-forge
            >> conda config -set channel_priority flexible

  Most of the time, it will freeze on Solving environment: failed with initial frozen solve. Retrying with flexible solve,
  One method to work around this is to create a conda environment:
  >> conda create -n cartopy
  >> conda activate cartopy:  
        Note that this will sometimes fail, and you need to close out the terminal and reload to save changes and properly activate.

  >> conda install cartopy
