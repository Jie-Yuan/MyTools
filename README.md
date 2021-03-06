<h1 align = "center"> Tools </h1>

---
http://bbs.bugcode.cn/t/77394

conda config --add channels intel

conda update conda

conda install -c intel daal-static 

pip install lightgbm --install-option=--nomp -U

https://anaconda.org/intel/daal-static
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
## [configparser][28]

## 虚拟环境
- [hatch][27]
- pyvenv

`rm -rf /var/tmp/*.swp`

https://blog.csdn.net/luanpeng825485697/article/details/78347433

https://www.zhihu.com/question/24590883

www.datacamp.com

## Pycharm
- `Settings → Editor → Auto-Import`

## Vim
- [行号高亮][29]

## 镜像
- [科大][88]
- [清华][888]
- [阿里源][26]
---
## 工具类
- [Linux][0]
    - [RPM][5]
- [Cygwin][8]
- [IntelPython][1]
- [Anaconda][2]
- [WinWheel][3]
- [Jetbrians注册码][6]
    - Pycharm默认设置Editor->File and Code Templates
- [Everything][9]
- [Matools][13]
- [Convert Excel sheet to MarkDown Table][15]
- [Pypi][18]
- [Pipenv][21]
- [FinalShell服务器管理][22]
- Notepad++
    - Notepad++ ->"运行"菜单->"运行"按钮
    ```
    cmd /k python "$(FULL_CURRENT_PATH)" & ECHO. & PAUSE & EXIT
    ```
 - 流程图
    - Xmind
    - [draw.io][23]: [桌面版][25]
    - [processon][24]
    
---
# 资源类
- [最新emoji][16]
- [emoji速查][17]
- [最流行数据集][12]
- [美团技术博客][4]
- [programcreek][20]: 函数查阅
---
## [Git][19]
- [git push][7]
- [git branch][14]
```
# 检验线上线下一致性
git status
git pull
git checkout
git add/rm ...
git checkout
git push
```
- Git常用命令速查
![Git常用命令速查][11]

---
## Pip
- Online: 镜像源加速
```
pip install --upgrade tensorflow -i https://pypi.tuna.tsinghua.edu.cn/simple
```

- 默认配置
    - linux: linux的文件在~/.pip/pip.conf
    - windows: windows在%HOMEPATH%\pip\pip.ini（新建）
```
[global]
trusted-host =  pypi.tuna.tsinghua.edu.cn
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
```

---

## [Jupyter][10]: A simple way to share Jupyter Notebooks
- IpynbShow: nbviewer.jupyter.org/github/Jie-Yuan+项目
- 多输出交互
```
echo 'c = get_config()
# Run all nodes interactively
c.InteractiveShell.ast_node_interactivity = "all"
c.NotebookApp.contents_manager_class="jupytext.TextFileContentsManager"' >> .ipython/profile_default/ipython_config.py
```
- 远程配置
```sh
jupyter notebook --generate-config
jupyter notebook password # 设置密码

# 写入文件~/.jupyter/jupyter_notebook_config.py
c.NotebookApp.ip='*'
c.NotebookApp.open_browser = False
c.NotebookApp.port = 8888 # 设置端口
c.NotebookApp.notebook_dir = '/yuanjie' # 设置目录
c.InteractiveShell.ast_node_interactivity = "all" # 设置多输出

```

---
## 常用包
```shell
pip install -U sklearn rgf_python lightgbm xgboost tensorflow keras keras-tqdm ml_metrics 
pip install -U seaborn scikit-plot pandas_summary sklearn_pandas missingno
pip install -U tpot auto_ml mlbox bayesian-optimization
thefuck bashsrc > alias fuck='eval $(thefuck $(fc -ln -1)); history -r'
```
---
## 数据库
- Hive
> sqlalchemy中hive的url形式: hive://localhost:port/database?auth=XX
```
pyhive
thrift
future
sasl
thrift_sasl
thriftpy
ply
sqlalchemy
```

https://blog.csdn.net/sijiaqi11/article/details/78601258



---
[0]: https://jaywcjlove.github.io/linux-command/
[1]: https://registrationcenter.intel.com/en/products/postregistration/?sn=CTGC-JS77PNXP&EmailID=313303303%40qq.com&Sequence=2053363&dnld=t
[2]: https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/
[3]: http://www.lfd.uci.edu/~gohlke/pythonlibs/
[4]: https://tech.meituan.com/
[5]: http://rpmfind.net/linux/rpm2html/search.php
[6]: http://xidea.online
[7]: http://www.cnblogs.com/qianqiannian/p/6008140.html
[8]: http://www.cygwin.com/
[9]: http://www.voidtools.com/
[10]: http://nbviewer.jupyter.org/
[11]: http://chuantu.biz/t5/162/1502091545x1884350018.jpg
[12]: http://archive.ics.uci.edu/ml/index.php
[13]: http://www.matools.com/
[14]: http://blog.csdn.net/arkblue/article/details/9568249/
[15]: https://github.com/fanfeilong/exceltk
[16]: https://emojipedia.org/
[17]: https://www.webpagefx.com/tools/emoji-cheat-sheet/
[18]: https://pypi.tuna.tsinghua.edu.cn/simple/
[19]: https://mp.weixin.qq.com/s/6kuJuJCng8AWVAlSYl1RrA
[88]: https://mirrors.ustc.edu.cn/
[888]: https://mirrors.tuna.tsinghua.edu.cn
[20]: https://www.programcreek.com/
[21]: http://blog.csdn.net/dream_allday/article/details/60467131
[22]: http://www.hostbuf.com/t/988.html
[23]: https://www.draw.io/
[24]: https://www.processon.com/
[25]: https://github.com/jgraph/drawio-desktop/releases
[26]: https://opsx.alibaba.com/mirror
[27]: https://github.com/ofek/hatch/blob/master/COMMANDS.rst
[28]: https://blog.csdn.net/shortwall/article/details/78615368
[29]: https://www.cnblogs.com/zl-graduate/p/5901090.html


[30]: http://ssl.picnet.com.au/xgboost/
