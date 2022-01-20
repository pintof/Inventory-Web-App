# Inventory-Web-App for Shopify Job Application
#Needs Python 3 installed to run
 
 #SETUP INSTRUCTIONS
 #(First change the direcory of the terminal to this directory where README, manage.py, and requirements.txt are present)
 
 #Step 1 - Create & activate a virtual environment
 #(Not necessary, but recommended to avoid dependancy version conflicts)
 
 #Install pipenv (if not already installed)
 pip install pipenv
 #Install django within the virtual environment
 pipenv install django
 #Launch the virtual environment
 pipenv shell

#Step 2 - Install Python dependencies
pipenv install -r requirements.txt
#Or if you don't want to run a virtual python environment then:
pip install -r requirements.txt

#Step 3 - Create SQLite databse, run migrations
python manage.py makemigrations
python manage.py migrate

#Step 4 - Run Django dev server
python manage.py runserver

#Step 5 - Visit web app
http://127.0.0.1:8000/todo
