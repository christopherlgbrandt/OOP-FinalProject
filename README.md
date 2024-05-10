# CSCI375Team

## Team Members:
* Bryan Bonilla
* Kyle Verbrugge
* Christopher Brandt

## Project Info: 
For our CSCI 375 final project we decided to work on the Packard Power Rankings website. The main things we hope to accomplish throughout this project are adding in various bug fixes to make the site run much smoother, redesigning the website UI to make it more friendly to end users, and potentially adding in new features. 


## Grades

### Judges

|  Bergen | Clayton | Average |
---|---|---|
| 35 | 39 | 37 |


## How to install packages and run the app

### Using Python Environment

```bash
git clone <this_repository>
cd <this_repository>
conda create -n <env_name> python=3.9
conda activate <env_name>
pip install -r requirements.txt
python manage.py migrate # apply db migrations
python manage.py runserver
```

### Using Docker

```bash
git clone <this_repository>
cd <this_repository>
$ bash run.sh
$ python manage.py migrate
# Depending on the above command you might have to run another 
# command to update the files with python manage.py makemigrations
$ python manage.py runserver 0.0.0.0:8000
```

## How to run test

```bash
python manage.py test
```