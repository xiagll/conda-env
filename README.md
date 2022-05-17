# conda-env
how to use conda environment (with Anaconda 3 in windows 10)

## Install conda
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

## Create and delete environmets
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

## Manage dependency package versions
### 1.create Requirements.txt document (for example Requirements.txt contains the following packages)
numpy(1.19.5)  
transformers(4.1.1)   
pandas(1.1.5)  
scipy(1.4.1)  
scikit-learn(0.24.0)  
torch(1.7.1)  
### 2.install all required packages
pip install -r requirements.txt
### 3.check the environment
python  
>>>import torch  
>>>import numpy  
>>>...  
>>> exit()
### 4. install pytorch in jupyter
conda install ipykernel
### 5. after opening jupyter
click the button: Kernel-Change kernel-Python[conda env:pytorch]  
then, display "Python[Conda env: PyTorch]" in the upper right corner


