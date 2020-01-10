# django-structure
Pre configured django project for making development fast, by cutting the initial setup time.

## Features
- Django version 2.2.8 (LTS)
- Ideal directory structure
- Manage multiple environments
- Logging configured

## Usage
- git clone https://github.com/nitinraturi/django-structure.git
- First, remove .git file and set your own repository later
```
rm -rf .git
```
- pip install -r requirements.txt
- create a file .env where manage.py is located and set your environment variables. Have a look sample file: .env-sample
- Generate SECRET_KEY using the command
```
python -c 'import random; print("".join([random.choice("abcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*(-_=+)") for i in range(50)]))'
```
- Now replace the SECRET_KEY value with the value generated in your terminal inside your .env file.
- Let's create required directories now, run
```
mkdir -p static/{css,js,img} static_cdn/{static_root,media_root} templates/{snippets,layouts} apps logs
```
- That's all, start developing...
