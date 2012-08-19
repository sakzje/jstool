Step-by-Step
============

Phase 1- Minimum Application
----------------------------

* use sqlite3 db
* run on AWS EC2 instance as a wsgi application
* use ``django-registration`` combined with ``email-as-username``
* use ``bootstrap`` for css

Features
........

* users can register and login
* home page lists jobs applied, last one first
* create/edit/delete/list Employer
* create/update/list Application
* create/edit/list Employer Diary

Data Modelling
..............

* Employer
  - user (foreign key)
  - name
  - description
  - website
  - contact1, contact2, contact3
* Application
  - employer (foreign key)
  - jobtitle
  - status
  - current action, date
  - next action, date
  - coverletter
  - resume
* Diary
  - employer (foreign key)
  - date
  - entry

Phase 1 - Step-by-Step
......................

* start project
* define sqlite3 db backend
* install ``email-as-username`` app; fix its problem with permissions
* 

Phase 2
-------

* use postgres db
