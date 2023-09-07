# conda_environments
Scripts to setup platform independent conda environments

## Testing Pytorch
In the activated environment:
  python -m torch.utils.collect_env  

Or, within Python:
  import torch
  torch.backends.cudnn.enabled
  torch.cuda.is_available()
  torch.cuda.get.device_name(0)

## Testing Tensorflow
  import tensorflow as tf
  tf.config.list_physical_devices('GPU')

## Troubleshooting
In case jupyter lab cannot connect to server, try updating prompt_toolkit:  
  conda update -c conda-forge prompt_toolkit

### Tensorflow Compatibility List
https://www.tensorflow.org/install/source#gpu

### Cuda Toolkit Version
https://anaconda.org/nvidia/cuda-toolkit

### List available cudnn versions
  conda search -c anaconda cudnn

### Pytorch Compatibility
https://pytorch.org/get-started/previous-versions/


### Pillow Compatibility
In case PIL does not work, it might be necessary to install it with pip.  
https://pillow.readthedocs.io/en/stable/installation.html


## Python 3.9 on WINDOWS 10
  conda create -y --name py39 python=3.9
  
  conda activate py39
  
  conda install -c "nvidia/label/cuda-11.3.1" cuda-toolkit
  
  conda install -c nvidia cudnn=8.2.1
  
  conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cudatoolkit=11.3 -c pytorch
  
  conda install tensorflow

...


## Python 3.10 on WINDOWS 10
conda create -y --name py310 python=3.10

conda activate py310

Install CUDA Toolkit 11.8.0
Install cuDNN 8.6
Get install cmd from https://pytorch.org/get-started/locally/



## Python 3.9 on UBUNTU
conda create -y --name py39 python=3.9

conda activate py39

conda install -y albumentations -c conda-forge

conda install -y scipy

conda install -y tensorflow-gpu

conda install -y pytorch torchvision torchaudio -c pytorch

conda install -y jupyter pandas seaborn -c conda-forge

conda install -y -c conda-forge natsort kneed pandas-profiling pyinstaller pyinstaller-hooks-contrib pytorch-model-summary shapely sweetviz tqdm umap-learn xgboost scikit-image scikit-learn scikit-optimize imbalanced-learn tabulate yapf skorch optuna celluloid scikit-learn-intelex pre-commit multicore-tsne opencv

conda install -y -c plotly plotly

pip install git+https://github.com/berni-lehner/zippee-ki-yay.git


## Python 3.10 on UBUNTU
conda create -y --name py310 python=3.10

conda activate py310

conda install -y -c conda-forge umap-learn albumentations jupyter pandas seaborn

conda install -y scipy

conda install -y tensorflow

conda install -y pytorch torchvision torchaudio -c pytorch


conda install -y -c conda-forge natsort kneed pandas-profiling pyinstaller pyinstaller-hooks-contrib pytorch-model-summary shapely sweetviz tqdm xgboost scikit-image scikit-learn scikit-optimize imbalanced-learn tabulate yapf skorch optuna celluloid scikit-learn-intelex pre-commit multicore-tsne opencv

conda install -y -c plotly plotly

pip install git+https://github.com/berni-lehner/zippee-ki-yay.git
