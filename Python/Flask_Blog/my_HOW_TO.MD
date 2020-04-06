# Setup
## env

0/ mkdir for project

1/ create  new env
python3 -m venv Project_name_here   # (--system-site-packages # for all packages available for new env)


2/ activate env
source Project_name_here/bin/activate

## files

0/ create file for app (any_name.py) THIS HOLDS ALL @app.route decorators for all file locations

# start flask server

1/ (command line:) export FLASK_APP=any_name.py

2/ flask run

# create structure
## create folders

1 / static (for css files)

2/ templates (for all templates)

## create structure files
1/ create layout.html  (bootstrap header, header, bootstrap body, etc, pl: google analitics)

2/ create home/about etc .html-s, inheriting static stuff from layout.html

3/ edit any_name.py @app.route decorators like this : 

@app.route("/home")
def home():
    return render_template('home.html')
    
![alt text](http://https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fthumb%2F9%2F97%2FClassic_smiley.svg%2F770px-Classic_smiley.svg.png&f=1&nofb=1)


