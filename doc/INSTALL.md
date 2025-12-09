## 安装 CARLA 0.9.11

## 设置
- 创建conda环境.
```
cd scppo
conda env create -f environment.yml --name carla
conda activate carla
easy_install ${CARLA_ROOT}/PythonAPI/carla/dist/carla-0.9.11-py3.7-linux-x86_64.egg
```
- 使用 wandb 进行实验记录，注册账户并登录。
```
wandb login
```

## 训练
CARLA库的文件名有所不同，所以，
```
easy_install ${CARLA_ROOT}/PythonAPI/carla/dist/carla-0.9.10-py3.7-linux-x86_64.egg
```
