There are various ways to create a virtual environment in python. Some of them are by using libraries such as: venv, virtualenvwrapper, pipenv, and conda.

## 1. venv
Usually `venv` library is already provided once you installed python. To activate the environment, firstly need to define the directory location.

**create new virtual environment**

without specific  python version (use default in system)
```
python -m venv my_venv
```
with specific  python version
```
python -m venv my_venv --python=--python=/path/to/python3.x/
```

**activate the environment**

in cmd windows
```
[my_venv directory]/bin/activate
```
in terminal linux
```
source [my_venv directory]/bin/activate
```

**deactivate the environment**
```
deactivate
```


## 2. virtualenvwrapper
`Virtualenvwrapper` library works based on the OS used.  As I am using Windows OS, I installed [virtualenvwrapper-win](https://pypi.org/project/virtualenvwrapper-win/). It is by default stored in single WORKON directory (for windows by default in drive C). Unlike venv, it can be activated without need to define the directory location.

**create new virtual environment**
without specific  python version (use default in system)
```
mkvirtualenv my_venv
```
with specific python version
```
mkvirtualenv my_venv --python=/path/to/python3.x/
```

**active the environment**
```
workon my_venv
```

**deactive the environment**
```
deactivate
```

**check all created environments**
```
lsvirtualenv
```

**define the WORKON directory**
```
set WORKON_HOME=C:\path\to\virtualenvs
```

## 3. pipenv

## 4. conda
If you install python in *Anaconda*, you can use `conda` command to manage and configure virtual environments. It is already there once completed the installation.

**create new virtual environment**
without specific  python version (use default in system)
```
conda create --name my_venv
```
with specific python version
```
conda create --name my_venv python=3.9
```

**active the environment**
```
conda activate my_venv
```

**deactive the environment**
```
conda deactivate
```

**check all created environments**
```
conda env list
```