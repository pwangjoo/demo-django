# README.md
Django starting guide for MacOS (M1).

### Prep
1. Usage of `pyenv`
  * 내장 Python을 별도의 목적으로 사용하면, MacOS의 성능이 저하될 수 있기 때문에, 별도의 Python 설치 / 사용을 권장함.
```zsh
% brew install pyenv #Homebrew installation
% pyenv versions #check installed version & current version
% pyenv install [VERSION] #latest 3.12.2 (on 24/03/14)
% pyenv uninstall [VERSION] #uninstall
% pyenv global [VERSION] #set global python
% pyenv local [VERSION] #set local python (genrates .python-version file)
```
1. Usage of `venv`
```zsh
% python -m venv .venv #generate virtual environment
% source .venv/bin/activate #activate
(.venv) % deactivate #deactivate
```
* Auto activation on VSCode
  1. Install VSCode Python package.
  1. `cmd`+`shift`+`p` > select Python: Select Interpreter

### Installation
```zsh
(.venv) % pip install django #install django
```

### Initializing
1. Generating new Django project
```zsh
(.venv) % django-admin startproject [DIRNAME] . #generate project
(.venv) % python manage.py runserver #run server
```
1. Easy start with NodeMon
  1. Install NodeMon.
  1. Add `package.json`.
  ```json
  {
    "scripts": {
      "start": "nodemon --exec python manage.py runserver"
    }
  }
  ```


### Running
```zsh
% npm run start #start development server
```