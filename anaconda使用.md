## Anconda 使用

#### Conda软件源配置

###### 1.查看现有源

`conda config --show-sources`

###### 2.添加国内源

`conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkg/free/`

`conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/`

###### 3.删除默认源

`conda config --remove channels defaults`

###### 4.设置搜索时显示通道地址

`conda config --set show_channels_urls yes`

###### 5.升级conda

`conda update conda` 

###### 6.更改配置文件更改源

`C:\Users\18857\.condarc`

#### 虚拟环境配置

###### 1.创建虚拟环境

`conda create -n normal python=3.8.0`

新的虚拟环境会被储存在你安装conda的目录的envs目录下

###### 2.激活环境

`activate normal`

###### 3.列出所有环境

`conda info -e`当前所激活环境前会有*标识

###### 4.切换到另一个环境

`activate name`

###### 5.注销当前环境

`deactivate`

###### 6.复制环境

`conda create -n 新环境name --clone 旧环境name`

###### 7.删除环境

`conda remove -n name --all`

#### 包管理

###### 1.查看已安装包

` conda list`

###### 2.使用conda命令安装包

`conda install 包名`

###### 3.通过pip命令安装包

`pip install 包名`

###### 4.移除包

`conda remove 包名`



