# Django Tutorial

## Steps

### 1. Install python and all it's environments. Check whether python and pip is install on your system run

```bash
python --version
and
pip --version
```

### 2. It is suggested to have a dedicated virtual environment for each Django project, and one way to manage a virtual environment is venv, which is included in Python. To check if the virtual environments is already installed type the following command

```bash
# for window
py -m venv yourEnvName

#for mac or unix system
python -m venv yourEnvName
```

#### This will set up a virtual environment, and create a folder named "yourEnvName"

#

#### To install the virtual environment if not already installed, type the following command

```python
pip install virtualenv
```

or

```python
python -m instll virtualenv
```

- Then you have to activate the environment, by typing this command:

```sh
# window
yourEnvName\Scripts\activate.bat
```

or

```bash
# for mac or unix system
source yourEnvName/bin/activate
```

### 3: Install Django project and App

- _**Note:** ` Remember to install Django while you are in the virtual environment!`_

To install Django type the following command

```sh
# Windows
py -m pip install Django
```

```sh
# Mac or unix system
python -m pip install Django
```
