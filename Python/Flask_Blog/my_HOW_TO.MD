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

# create main folders

1 / static (for css files)
2/ templates (for all templates)


