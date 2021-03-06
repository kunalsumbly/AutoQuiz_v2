# AutoQuiz
Master of Science Project code, using [Flask](http://flask.pocoo.org/).

[Thesis](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2018/EECS-2018-54.html) available online.

## Dependencies

* Based on [Flask](http://flask.pocoo.org/) framework
* Front-end using [JQuery](https://jquery.com/) and [Bootstrap](https://getbootstrap.com/)
* Login system handled by [Flask-Login](https://flask-login.readthedocs.io/en/latest/)

## Simplified maintnance:

**0.** Initialize database by running ***sh init_db.sh*** on mac, or ***sqlite3 auto_quiz.db < schema.sql*** followed by ***python init_db.py*** in any other environment. 

Note: this initialization will clear the user data you already have. In fact, you might want to update using only ***python init_db.py***.

**1.** When adding a question to the system:
- create a new xml file under ***./static/dataset/*** with the given format of other existing .xml files;
- if involve new skill, log it by adding new key-value pairs in variable ***skill_map*** in ***init_db.py***;
- run script ***update_db_skill_question.py***

**2.** About the environment:

I used Python 2.7 back then.

Run by ```python auto_quiz.py```.
