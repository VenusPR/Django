# DjangoBlog

基于`python3.5`和`Django1.10`的博客。   

[![Build Status](https://travis-ci.org/liangliangyy/DjangoBlog.svg?branch=master)](https://travis-ci.org/liangliangyy/DjangoBlog) [![Coverage Status](https://coveralls.io/repos/github/liangliangyy/DjangoBlog/badge.svg?branch=master)](https://coveralls.io/github/liangliangyy/DjangoBlog?branch=master) [![Requirements Status](https://requires.io/github/liangliangyy/DjangoBlog/requirements.svg?branch=master)](https://requires.io/github/liangliangyy/DjangoBlog/requirements/?branch=master)  [![license](https://img.shields.io/github/license/liangliangyy/djangoblog.svg)]() [![GitHub release](https://img.shields.io/github/release/liangliangyy/djangoblog.svg)]() [![python3.5](https://img.shields.io/badge/python-3.5-brightgreen.svg)]() [![django1.10](https://img.shields.io/badge/django-1.10-brightgreen.svg)]()     

## 安装
使用pip安装：  
`pip install -r requirements.txt`

如果你没有pip，使用如下方式安装：    
OS X / Linux 电脑，终端下执行:  

    curl http://peak.telecommunity.com/dist/ez_setup.py | python
    curl https://raw.github.com/pypa/pip/master/contrib/get-pip.py | python

windows电脑：  
 下载 http://peak.telecommunity.com/dist/ez_setup.py 和 https://raw.github.com/pypa/pip/master/contrib/get-pip.py 这两个文件，双击运行。  


## 运行

 修改`DjangoBlog/setting.py` 修改数据库配置，如下所示：

     DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.mysql',
            'NAME': 'djangoblog',
            'USER': 'root',
            'PASSWORD': 'password',
            'HOST': 'host',
            'PORT': 3306,
        }
    }

### 创建数据库

 终端下执行:  

    ./manage.py makemigrations
    ./manage.py migrate  
### 创建测试数据
终端下执行:  

    ./manage.py create_testdata
### 开始运行：
 执行：  
 `./manage.py runserver`





 浏览器打开: http://127.0.0.1:8000/  就可以看到效果了。
