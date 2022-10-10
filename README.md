# wagtail-space-liveblog

## Set Up Locally

`python -m venv venv`

`source venv/bin/activate`

`python manage.py migrate`

`python manage.py createcachetable`

`python manage.py createsuperuser`

`psql -U postgres`

`CREATE DATABASE wagtail_space_liveblog;`


## Run Locally

open new terminal
```
$ source venv/bin/activate
```

```
$ python manage.py runserver
``` 
keep running in open terminal

open new terminal 

```
$ ngrok http 8000
```
keep running in terminal

open new terminal

```
$ docker network create redis-network`
```
``` bash
$ docker run --rm \
    --network=redis-network \
    --name=redis-server \
    -p 6379:6379 \
    redis
```
keep running in terminal

follow instructions to set up [wagtail live instructions - slack integration](https://wagtail.github.io/wagtail-live/getting_started/receivers/setup_slack/)




```Python 
# Error

{'ok': False, 'error': 'missing_scope', 'needed': 'users:read', 'provided': 'channels:history,files:read,metadata.message:read'}

# SOLUTION

Create the old version of the application. Slack updated their API Feb 2021.

```

## Deploying to...

### Azure

### Heroku

### Digital Ocean