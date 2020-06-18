# Docker-webapp-Python-Application


## 1. Create a docker image 

> $docker run ubuntu

> $docker run -it ubuntu bash


## 2. Setting Up Python 3 in the container

Ubuntu 20.04 and other versions of Debian Linux ship with Python 3 pre-installed. To make sure that our versions are up-to-date, let’s update and upgrade the system with the apt command :

> apt update

> apt -y upgrade


Once the process is complete, we can check the version of Python 3 that is installed in the system by typing:

> python3 -V 



To manage software packages for Python, let’s install pip.

> apt install -y python3-pip


Here I will use flask , so to install it run the below command.

> pip3 install flask


Install all the dependencies required.

> apt-get install -y python3 python-setuptools python-dev build-essential python3-pip python3-mysqldb


* copy source code from app.py
* cat > /opt/app.py
* paste the code and exit



## 3. Start Web Server

> FLASK_APP=app.py flask run --host=0.0.0.0


## 4. Run the Application

```
http://<IP>:5000                            => Welcome
http://<IP>:5000/how%20are%20you            => I am good, how about you?
```








