# Kamerka GUI
- https://github.com/woj-ciech/Kamerka-GUI

## Setup and Installation: 

```
sudo apt install redis redis-server
git clone https://github.com/woj-ciech/Kamerka-GUI/
pip3 install -r requirements.txt
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver
```

1. Execute this command in the main directory: ```celery worker -A kamerka --loglevel=info```
2.  Intialize Celery: ```celery --app kamerka worker```
3.  Karmerka should be running by going to the following URL: http://localhost:8000/
