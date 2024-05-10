# CSCI375Team

## Team Members:
* Bryan Bonilla
* Kyle Verbrugge
* Christopher Brandt

## Project Info: 
For our CSCI 375 final project we decided to work on the Packard Power Rankings website. The main things we hope to accomplish throughout this project are adding in various bug fixes to make the site run much smoother, redesigning the website UI to make it more friendly to end users, and potentially adding in new features. 


## Self Grades
Chris Brandt - 75% | I decided to give myself this grade on the project because while I really did try to work hard and make sure that I helped my teammates wherever I could, I still in large part failed to make a big contribution on the project overall. Looking back on it I realized that I jumped into the project far to fast without asking enough questions, if I had known the state of this project at the start of the semester I would have heavily tried to push us in a different direction. However, I think that this project really turned out to really be something that helped me learn a lot. I saw how much harder it becomes to communicate between a larger group, and how important it is to fully understand the scope of the project when taking on someone elses work. Overall though I worked hard creating those memory profiles, and doing what I could to optimize how many allocations each python file made. Along with this I believe that me and my teammates did a good job on the student showcase presentation, and that the website will be in good hands with it's future developers.
### Judges

|  Bergen | Clayton | Average |
---|---|---|
| 35/45 | 39/45 | 37 |


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
bash run.sh
python manage.py migrate
# Depending on the above command you might have to run another 
# command to update the files with python manage.py makemigrations
python manage.py runserver 0.0.0.0:8000
```

## How to run test

```bash
python manage.py test
```
