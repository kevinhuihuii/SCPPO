## Install CARLA
- Install CARLA 0.9.11 release

## Setup scppo
- create conda environment.
```
cd scppo
conda env create -f environment.yml --name carla
conda activate carla
easy_install ${CARLA_ROOT}/PythonAPI/carla/dist/carla-0.9.11-py3.7-linux-x86_64.egg
```
- We use wandb for logging, please register a free account and login to it.
```
wandb login
```

## For RL training
Our RL training crashed more often on CARLA 0.9.11 than on CARLA 0.9.10.1.
So for RL training we create an environment with the CARLA 0.9.10.1 release. 

the filename of the CARLA library is different
```
easy_install ${CARLA_ROOT}/PythonAPI/carla/dist/carla-0.9.10-py3.7-linux-x86_64.egg
```
