# conda_environments
Scripts to setup platform independent conda environments

## Python 3.9 on UBUNTU
conda create -y --name py39fullstack python=3.9

conda activate py39fullstack

conda install -y albumentations -c conda-forge

conda install -y tensorflow-gpu

conda install -y pytorch torchvision torchaudio -c pytorch

conda install -y jupyter pandas seaborn -c conda-forge

conda install -y -c conda-forge natsort kneed pandas-profiling pyinstaller pyinstaller-hooks-contrib pytorch-model-summary shapely sweetviz tqdm umap-learn xgboost scikit-image scikit-learn imbalanced-learn tabulate yapf skorch optuna celluloid scikit-learn-intelex pre-commit

conda install scipy

conda install -y -c plotly plotly

pip install git+https://github.com/berni-lehner/zippee-ki-yay.git
