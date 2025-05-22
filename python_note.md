# 学习笔记

## 1. conda
### 1） 下载
国内到清华园镜像下载
国外不需要
![](pics/GitHub.png)

### 2） 安装
- 不要安装到C盘，保持C盘的整洁，有助于系统的稳定运行

### 3） 使用
- 初始化：打开 `conda prompt`，输入命令：`conda init`，会添加`conda`的系统环境变量

- 修改系统powershell的执行策略：设置-系统-开发者选项-powershell-更改执行策略：打开  
这样的话就可以在windows的powershell里直接使用conda命令了
- 简单介绍一下用法：  
a. `conda --version` 查看安装版本  
b. `conda --help` 查看帮助文件。（大多数命令行工具都可以使用这个命令查看帮助文件，了解这些命令的基本使用方法）


### 4） 常用命令
- `conda create -n env_name python=3.10` 创建一个新的虚拟环境，env_name是你自己定义的环境名称
- `conda activate env_name` 激活虚拟环境
- `conda deactivate` 退出虚拟环境
- `conda env list` 查看所有的虚拟环境
- `conda remove -n env_name --all` 删除虚拟环境
- `conda install package_name` 安装包（但是比较推荐使用`pip`）
- `conda update package_name` 更新包
- `conda remove package_name` 删除包
- `conda list` 查看当前环境下安装的所有包
- `conda update conda` 更新conda

### 5） 常用源
- 清华源
```bash
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --set show_channel_urls yes
```
**注意**
- python的环境需要相互隔离，这样的话，环境之间就不会相互污染

## 2. pip
### 1） 修改镜像源

### 2） 常用命令
- `pip install package_name` 安装包
- `pip uninstall package_name` 卸载包
- `pip list` 查看当前环境下安装的所有包


## 3. git
### 1） 下载
国内同样用清华园

### 2） 安装
- 非系统盘
- 一般默认即可，选`recommended`的选项。如果使用`vscode`作为默认编辑器，需选择对应选项


### 3） 使用
- `git --version`
- `git --help`
- 需要先到`github`建立项目，然后使用`git clone`命令将项目克隆到本地
- `git init` 初始化本地仓库

### 4） 常用命令


### 5） 配置git
- `git config --global user.name "your name"` 设置用户名
- `git config --global user.email "your email"` 设置邮箱
- `git remote add origin <url>` 添加远程仓库, `origin`是远程仓库的名称，`url`是远程仓库的地址
- `git push -u origin master` 推送代码到远程仓库  
`master`是分支名称, 如果是`main`分支就改成`main`  
`-u`参数表示将本地分支与远程分支关联起来，以后可以直接使用`git push`命令推送代码


