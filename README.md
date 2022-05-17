# conda-env
how to use conda environment (with Anaconda 3 in windows 10)

## install conda
### 1.set the path (after installing Anoconda 3, you need only to set these paths)
C:\Users\111111\Anaconda3
C:\Users\111111\Anaconda3\condabin
C:\Users\111111\Anaconda3\Library\bin
### 2.check the version
conda --version
(if the conda version shows, it is installed)
### 3.common commands of conda
conda env list
conda list
conda search numpy
conda install numpy
conda uninstall numpy
conda update numpy
conda clean -p (delete useless packages)
conda clean -y --all (delete all packages and cache)
conda clean -t (delete tar package)

## create and delete environmets
### 1.Create virtual environment
conda create -n [name] python==3.6
### 2.Activate virtual environment
conda activate [name]
### 3.Check the list
conda list
### 4.Exit virtual environment
conda deactivate
### 5.delete environment
conda remove -n [name] --all
