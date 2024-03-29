# Tested on WSL - Ubuntu

## Install virtual env if not available

```
 sudo apt install python3-virtualenv
```

## Activate the virtual env
```
source appEnv/bin/activate
```


##  First install the dependencies

```
pip install -r requirements.txt
 ```

 ## Run the Fast API app

 ```

 uvicorn --port 8000 --host 127.0.0.1 main:app --reload

 ```

 ## Testing  -- note that the token string is secret
 ```
http://127.0.0.1:8000/docs 
 ```

 ## Create a deployment configuration procfile for Heroku.

 * Procfile is a heroku specific file and is read by the deployment configurations .
 * Heroku automatically looks for the presence of procfile and executes the commands located in it.


# install heroku cli on WSL - Ubuntu
* https://devcenter.heroku.com/articles/heroku-cli 

# See  in Action 
*  git push heroku master


# Python version

```
python -V
Python 3.8.10
```

# Debugging heroku logs from cli
```
heroku logs --tail
```

Reference - https://devcenter.heroku.com/articles/logging#view-logs 


# WSL2 
```
Using WSL2 - Windows Subsystem for Linux
Installing net-tools for route, ifconfig, etc.
Note that ifconfig is depreciated now, so use ip a
sudo apt install net-tools

Install docker on WSL2
Docker Desktop WSL 2 backend
https://docs.docker.com/desktop/windows/wsl/

```

## Testing 
https://jshreyas-fastapi-app.herokuapp.com/docs 