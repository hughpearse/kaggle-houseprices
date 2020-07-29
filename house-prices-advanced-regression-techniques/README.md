# kaggle-houseprices

# Data
https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data

# Program Usage
```bash
foo@bar:~$ virtualenv sandbox
foo@bar:~$ virtualenv -p $(which python3) sandbox
foo@bar:~$ source sandbox/bin/activate
foo@bar:~$ pip install -r requirements.txt 
foo@bar:~$ chmod 700 ./run.py
foo@bar:~$ python3 ./run.py dev
foo@bar:~$ deactivate
```

# Dockerised Environment
You will need to install Docker available for [Mac](https://hub.docker.com/editions/community/docker-ce-desktop-mac) or [Windows](https://hub.docker.com/editions/community/docker-ce-desktop-windows).
Next you might need to increase the available RAM on the containers to 8GB.


```bash
foo@bar:~$ docker build -t "fedora26-python3:1" -f ./Dockerfile . # Build docker image
foo@bar:~$ docker image ls # List docker images
foo@bar:~$ docker run --name f26-py3-container -t -d fedora26-python3:1 bash # Deploy and run container
foo@bar:~$ docker ps -a # List docker containers
foo@bar:~$ docker cp ./run.py f26-py3-container:/opt/app-root/src # Copy files on to container
foo@bar:~$ docker exec -i -t -u root f26-py3-container /bin/bash # Log in to container
root@f26:~# exit # Leave the container
foo@bar:~$ docker stop f26-py3-container # Turn off the container
```
