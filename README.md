# Django-Email-Sender
Send email from Gmail Id in Django using HTML Template

## Pre-Requisites
- Python 3.7
- Pip
- Git

## Steps to run:
- Clone the project using the command "git clone https://github.com/sukanya-pai/Django-Email-Sender.git"
- In PipFile, the dependencies are mentioned. It is recommended to run the app inside a virtual environment to avoid conflict of existing dependencies.
  - Run the command "pip install pipenv"
  - Run "pipenv shell". Creates virtual env
  - Run "pipenv install". Installs dependencies from the PipFile and creates PipFile.lock
  - Run "python manage.py runserver" to start the server
- Make changes in the [views.py](https://github.com/sukanya-pai/Django-Email-Sender/blob/master/email_project/email_proj/views.py) file inside the send_mail() method to add your mail address and the recipients mail address accordingly.
- Make changes in the [settings.py](https://github.com/sukanya-pai/Django-Email-Sender/blob/master/email_project/email_project/settings.py) file with your gmail id and your gmail id's password. 
  - Since this is a demo project, the password is written directly in settings.py. For security reasons of your account, it is recommended you store the password in key vault or encrypt it and then host the application or push your changes to GitHub.


## Mandatory changes to be done in Host Gmail account
- Go to https://myaccount.google.com/security
- Scroll till you find "Less secure app access"
- Here you will find that the status is Off. You need to turn this to On State. 
Only if you follow the above steps, then you can send mail from your Gmail account using your django code. 
