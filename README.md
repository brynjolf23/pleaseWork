Description:
Enter accurate information into the search forms. The homepage form searches for any twitter account and displays the last 30 tweets and a graph showing likes vs time.
Users may register for a mailing list.

If you get an internal server error then the listing you typed does not exist. This is espically true when using heroku. 
The others meaning flask and gunicorn have problems with tkinter hence getting an internal server error(500) does not necessarily mean the listing you are requesting is not there.

Before trying to run you should:
-install git with "sudo apt install git" or install with your system's alternative.


For running on flask localhost:
-Clone my repository with git clone repository link.
-cd to the directory you cloned it to
-Create a virtual environment with python3 -m venv venv
-NB: Do "sudo apt-get install python3-venv" if you get the virtual enviromnment was not created successfully because ensurepip is not available error.
-Once venv is created do "source venv/bin/activate"
-install requirements with "pip3 install -r requirements.txt"
-install my sql client with "sudo apt-get install libmysqlclient-dev"
-install tkinter with "sudo apt-get install python3-tk"
-"flask run" to run the application on localhost

For running with gunicorn:
-Clone my repository with git clone repository link.
-cd to the directory you cloned it to
-Create a virtual environment with python3 -m venv venv
-NB: Do "sudo apt-get install python3-venv" if you get the virtual enviromnment was not created successfully because ensurepip is not available error.
-Once venv is created do "source venv/bin/activate"
-install requirements with "pip3 install -r requirements.txt"
-install my sql client with "sudo apt-get install libmysqlclient-dev"
-install tkinter with "sudo apt-get install python3-tk"
-"gunicorn: wsgi:app" to run the application

SOME STUFF ABOUT FLASK LOCALHOST AND GUNICORN:

After switching tabs, you may get the error 500, when trying to find a listing, to solve this, you have to restart the app.

Do not use the back button on the browser. Instead you have to physically alter the link for it to work. E.g if you want to go back the the home page from http://127.0.0.1:5000/form you have to physically change it to http://127.0.0.1:5000 

If ever get 500 error you should go to http://127.0.0.1:5000 or what ever the original link was or restart the server by doing ctrl + c in the terminal and retyping the last command of the respective runtype.

Deploying on heroku:
-Clone my repository with git clone repository link.
-cd to the directory you cloned it to
-in a terminal type "heroku login"
-"git init"
-"git add --all"
-"git commit -m "Initial""
-"heroku create"
-"git push heroku master"
-"heroku open"

If you want to see what the online database looks like:
Please do not fuck with it.

Database details
['MYSQL_HOST'] = 'remotemysql.com'             
['MYSQL_USER'] = 'KfZiCHimwl'
['MYSQL_PASSWORD'] = '3UfECxWJRp'
['MYSQL_DB'] = 'KfZiCHimwl'

Instructions:
All user information and channels are saved to an online database on remotemysql

Username for PHPmyadmin=KfZiCHimwl
Password for PHPmyadmin=3UfECxWJRp
