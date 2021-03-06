# Setup

As the first of the demos, a bit of setup is required here.

* You need a server (your laptop, a virtual server in AWS or Digital Ocean)
* Install Python and all depencies
* Maybe you are excited, but take a little time to set yourself up for success before you continue forward
  * How will you organize your changes?
  * What editor will you use?
  * What are natural stopping points for you?
  
  
## Python Setup

These setup commands will be helpful.  These particular examples were built on Mac OSX with Python 3.6
* ```pip3 install --upgrade pip``` to upgrade your version of pip.
* ```pip3 install cookiecutter -U --user``` to add the package dependency manager used in this course
* ```python3 -m venv --copies .env``` Virtual environment setup with .env flag for Pycharm venv awareness on OSX.



If you are using Anaconda, this is an easy way to start your project in a conda virtual environment:

```server:talkpython phil$ conda create --name talkpython1 pyramid
Fetching package metadata .........
Solving package specifications: .

Package plan for installation in environment /Users/phil/anaconda3/envs/talkpython1:

The following NEW packages will be INSTALLED:

    openssl:           1.0.2l-0     
    pastedeploy:       1.5.2-py36_1 
    pip:               9.0.1-py36_1 
    pyramid:           1.5.7-py36_0 
    python:            3.6.2-0      
    readline:          6.2-2        
    repoze.lru:        0.6-py36_0   
    setuptools:        27.2.0-py36_0
    sqlite:            3.13.0-0     
    tk:                8.5.18-0     
    translationstring: 1.3-py36_0   
    venusian:          1.0-py36_0   
    webob:             1.6.1-py36_0 
    wheel:             0.29.0-py36_0
    xz:                5.2.2-1      
    zlib:              1.2.8-3      
    zope:              1.0-py36_0   
    zope.deprecation:  4.2.0-py36_0 
    zope.interface:    4.3.3-py36_0 

Proceed ([y]/n)? y

repoze.lru-0.6 100% |################################| Time: 0:00:00 599.19 kB/s
translationstr 100% |################################| Time: 0:00:00   3.40 MB/s
venusian-1.0-p 100% |################################| Time: 0:00:00   4.58 MB/s
webob-1.6.1-py 100% |################################| Time: 0:00:00   3.33 MB/s
zope-1.0-py36_ 100% |################################| Time: 0:00:00   2.97 MB/s
pastedeploy-1. 100% |################################| Time: 0:00:00  19.46 MB/s
zope.deprecati 100% |################################| Time: 0:00:00  16.36 MB/s
zope.interface 100% |################################| Time: 0:00:00   5.54 MB/s
pyramid-1.5.7- 100% |################################| Time: 0:00:00   5.48 MB/s
#
# To activate this environment, use:
# > source activate talkpython1
#
# To deactivate an active environment, use:
# > source deactivate
#
(talkpython1) server:talkpython phil$ cookiecutter https://github.com/Pylons/pyramid-cookiecutter-starter
project_name [Pyramid Scaffold]: My Web App
repo_name [my_web_app]: 
Select template_language:
1 - jinja2
2 - chameleon
3 - mako
Choose from 1, 2, 3 [1]: 2

===============================================================================
Documentation: https://docs.pylonsproject.org/projects/pyramid/en/latest/
Tutorials:     https://docs.pylonsproject.org/projects/pyramid_tutorials/en/latest/
Twitter:       https://twitter.com/PylonsProject
Mailing List:  https://groups.google.com/forum/#!forum/pylons-discuss
Welcome to Pyramid.  Sorry for the convenience.
===============================================================================

Change directory into your newly created project.
    cd my_web_app

Create a Python virtual environment.
    python3 -m venv env

Upgrade packaging tools.
    env/bin/pip install --upgrade pip setuptools

Install the project in editable mode with its testing requirements.
    env/bin/pip install -e ".[testing]"

Run your project's tests.
    env/bin/pytest

Run your project.
    env/bin/pserve development.ini

(talkpython1) server:talkpython phil$ tree
.
├── CHANGES.txt
├── MANIFEST.in
├── README.txt
├── development.ini
├── my_web_app
│   ├── __init__.py
│   ├── static
│   │   ├── pyramid-16x16.png
│   │   ├── pyramid.png
│   │   └── theme.css
│   ├── templates
│   │   ├── layout.pt
│   │   └── mytemplate.pt
│   ├── tests.py
│   └── views.py
├── production.ini
├── pytest.ini
└── setup.py

3 directories, 15 files
```

# Helpful Links

* [Michael Kennedy's official Repo](https://github.com/mikeckennedy/python-for-entrepreneurs-course-demos.git)

---
_This is NOT an official part of the course.  Just one learner taking notes._
