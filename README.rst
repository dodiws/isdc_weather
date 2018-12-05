=======
weather
=======

Dashboard and api weather modules.
Mandatory Module for ASDC

Quick start
-----------

1. Add "weather" to your DASHBOARD_PAGE_MODULES setting like this::

   DASHBOARD_PAGE_MODULES = [
       ...
       'weather',
   ]

   If necessary add "weather" in (check comment for description): 
       QUICKOVERVIEW_MODULES, 
       MAP_APPS_TO_DB_CUSTOM

   For development in virtualenv add WEATHER_PROJECT_DIR path to VENV_NAME/bin/activate:
       export PYTHONPATH=${PYTHONPATH}:\
       ${HOME}/WEATHER_PROJECT_DIR

2. To create the weather tables:

   python manage.py makemigrations
   python manage.py migrate weather --database geodb
