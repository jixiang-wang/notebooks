# notebooks
存储notebooks的笔记

32 GB内存

2个CPU核心

40分钟不活动超时

最多10 GB的永久磁盘空间

https://notebooks.gesis.org


2种配置文件：

1、requirements.txt

1）安装pip-tools

```
$ source /path/to/venv/bin/activate

(venv)$ python -m pip install pip-tools
```

2）在requirements.in或setup.py中添加相关依赖，如：

requirements.in：

```
numpy
pandas
matplotlib==3.3.0
seaborn==0.10.1
scikit-learn==0.23.2
qgrid==1.3.1
catboost==0.24
xgboost==1.1.1
tqdm
lightgbm
pycaret
```
3)生成requirements.txt：
```
pip-compile
```


一般从安装依赖的命令：

```
pip install -r requirements.txt
```


详情可参见链接：https://github.com/jazzband/pip-tools/


2、environment.yml

```
$ source /path/to/venv/bin/activate
conda env create -f environment.yml
```


