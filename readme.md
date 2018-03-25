# 基于Django的个人学习网站

这是我学习后端开发的第一个小项目，实现的功能是个人笔记。正好以这个作业学习了 Django 和 Web 开发。

已实现功能：

1. 一个无限可能的主页
2. 增加主题，增加具体条目
3. 注册用户
4. 登录登出用户
5. 用户只能看到各自的数据
6. 后台管理

## 环境及依赖

这个网站使用 Python 3.6.4 开发，其他版本没有测试过。Django 使用当前2.x，使用旧版本1.x需要修改部分代码。推荐使用 [virtualenv](https://virtualenv.readthedocs.org/) 来搭建环境。

```
Python (3.6.4)
Django (2.0.3)
django-bootstrap3 (9.1.0)
```
## 配置

如果部署网站，需要做如下配置

```python

```

数据库默认使用 SQLite，可以修改成 MySQL

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': os.path.join(PROJECT_PATH, 'db.sqlite3'),
    }
}
```

本地调试网站，可以运行如下命令

```python
python manage.py runserver
```

## 网站效果图

### 首页

![img1.jpg](doc/img1.jpg "")

----------

### 主题页

![img2.jpg](doc/img2.jpg "")

----------

### 详细条目页

![img3.jpg](doc/img3.jpg "")

----------
### 增加，编辑页
![img4.jpg](doc/img4.jpg "")
![img5.jpg](doc/img5.jpg "")
![img6.jpg](doc/img6.jpg "")

