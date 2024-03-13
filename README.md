# README.md
This is a demo repository for Django project.

### Before starting
1. Usage of `pyenv`
```zsh
% brew install pyenv #installation
% pyenv versions #check installed version
% pyenv version #check current version
% pyenv install [version] #latest 3.12.2
% pyenv uninstall [version]
% pyenv global [version] #set global python
% pyenv local [version] #set local python (genrates .python-version file)
```
1. Usage of `venv`
```zsh
% python -m venv .venv #generate virtual environment
% source .venv/bin/activate #activate
(.venv) % deactivate #deactivate
```

### Installation
```zsh
(.venv) % pip install django #install django
```

### Initializing
```zsh
(.venv) % django-admin startproject [folder-name] . #generate project
(.venv) % python manage.py runserver #run server
```

### Running
```zsh
% npm run start #start development server
```