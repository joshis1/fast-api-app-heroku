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

 