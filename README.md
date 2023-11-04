# How to setup Python Virtual Environment (venv)
## Assume that you Python installed on your computer
## if not
```bash
brew install python
```
if you don't have brew, please install from 
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

If you are on Linux, install python with apt-get

## if yes, Let's start with venv

Create a project directory

```bash
mkdir myproject
cd myproject
```
Open in VScode

```bash
python -m venv venv
```
here last venv is the name of your environment, you can give any name.

now, activate the environment
```bash
source venv/bin/activate
```

You can deactivate the environment by 
```bash
deactivate
```

If you want to set different Python versions in your environment, you need to have Python Version Manager
```bash
brew update
brew install pyenv
pyenv --version

pyenv install 3.8
pyenv install 3.10
pyenv install 3.11

pyenv --versions

```
to set your global version of python
```bash
pyenv global 3.8
```

to set your local version of python in your project

```bash
cd myproject
pyenv local 3.10
```
