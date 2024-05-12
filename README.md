# OOP-FinalProject

## Packard Power Rankings Repository
https://github.com/packardpowerrankings/packardrankings
Developments have been made to the HS-Football branch.

## Team Members:
* Bryan Bonilla
* Kyle Verbrugge
* Christopher Brandt

## Project Info: 
For our CSCI 375 final project we decided to work on the Packard Power Rankings website. The main things we hope to accomplish throughout this project are adding in various bug fixes to make the site run much smoother, redesigning the website UI to make it more friendly to end users, and potentially adding in new features. 

## Grading

### Judge Grading

| Jeremy Bergen | Clayton Johnson | Average |
|---|---|---|
| 35/45 | 39/45 | 37 |

### Group Self-Grading

|  Section | Self-Grade | Justification |
---|---|---|
| Use of Fundamental OOD Concepts | 5/5 | The whole project is object oriented with Classes, Inheritance, Getters and Setters |
| Use of at least 3 Design Patterns | 2/5 | Design patterns were present within the project, but we could've done better to make them a more integral part of the project and presentation. |
| Testing for Correctness | 3/5 | Test coverage wasn't great, but there were a lot of files that weren't tested by the previous developers. |
| Documentations | 5/5 | We documented every new change and why that change was added. The documentation was done in Microsoft Teams and on a Word document. |
| Software Management | 5/5 | How we managed the software was through Microsoft teams with weekly meetings where individuals disclosed their progress and future developments. GitHub was also really good for managing who did what on the website as the tasks were given through issues. |
| Teamwork | 5/5 | The team communicated well and used one another for assistance when needed. There wasn't any case where one teammate's work collided with another's. |
| Project Requirements | 3/5 | The project was more than adequately challenging for a Sophomore-Junior student. Due to its complexions, there were a few setbacks which resulted in poor execution of fixing/improving the website. |
| Team Presentation | 5/5 | Each member of the team did a great job presenting visually and orally. Each member contributed a fair share to the presentation. |
| 4+1 Views | 4/5 | We had the 4+1 views completed, although there are couple that can be confusing and might not fall align with what's in the textbook. It was also difficult to come up with proper 4+1 diagrams due to the scope of the project. |
| Bonus: Above and Beyond | 6/10 | The project was very much like the real-world, so it provided everyone with hands-on experience. We worked directly with a client. Deployment was required to display the developments on the actual website. A database was used aswell. |
| Overall Score | 38/45 | N/A |

## Individual Contributions
### Chris Brandt - 75% - 
I decided to give myself this grade on the project because while I really did try to work hard and make sure that I helped my teammates wherever I could, I still in large part failed to make a big contribution on the project overall. Looking back on it I realized that I jumped into the project far to fast without asking enough questions, if I had known the state of this project at the start of the semester I would have heavily tried to push us in a different direction. However, I think that this project really turned out to really be something that helped me learn a lot. I saw how much harder it becomes to communicate between a larger group, and how important it is to fully understand the scope of the project when taking on someone elses work. Overall though I worked hard creating those memory profiles, and doing what I could to optimize how many allocations each python file made. Along with this I believe that me and my teammates did a good job on the student showcase presentation, and that the website will be in good hands with it's future developers.

All contributions can be found on the showcase presentation. Below is an overview of what we all did.

### Kyle Verbrugge
Google Analytics: Added a code snippet to each generated HTML headers. This code snippet connects to Google Analytics which displays data on the website such as hit counters, demographics, engagement, and growth statistics.

Crontab Back-Ups: Added a backup system on the Lightsail server so that situations like what happened this semester can be easily avoidable. There are two types of backups: temporary weekly backups and permanent (unless deleted) monthly backups.


### Bryan Bonilla

I wasn't able to contribute much to the project as would have liked. I was trying to spend time working on improving the input validation for entering games through a csv file. What I was able to get done was just a couple of changes to the csv_import method on the entering games admin page, and I created a django test class to try to see if I was going on the right track.

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
