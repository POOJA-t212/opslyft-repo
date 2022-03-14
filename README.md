

################Please follow below steps to complete my assignment.##############
############


# Flask-Docker-App

## Set up & Installation.

### 1 .Clone/Fork the git repo and create a virtual environment 


1. clone any flask sample repo.

```
### 2 .Activate the environment
          
```. venv/bin/activate```
or
```source venv/bin/activate```


### 3 .Install the requirements

Applies for windows/macOS/Linux

```
pip install -r requirements.txt
```

### 5. Run the application
`python app.py`

# OR

## Create a new application from scratch

### 1. Create a directory with a name **"Flask-Docker-App"**
`mkdir Flask-Docker-App`

### 2. Navigate to the newly created directory

`cd Flask-Docker-App`

### 3. Create a virtual environment


**macOS/Linux**

`python3 -m venv venv`

### 4. Activate the environment
          
**Windows** 

```venv\Scripts\activate```
          
**macOS/Linux**

```. venv/bin/activate```
or
```source venv/bin/activate```

### 3 .Install Flask

`pip install Flask`

### 4. Create the required files
Create two files; **app.py** and **Dockerfile**

`touch app.py Dockerfile`

###Thanks you From POOJA




###########screenshot of an flask application running in docker container and opening in browser####

Once I build the docker image using below command 
#docker build --tag flask-py-docker-2 .
this has created my images in my local ..please see below.
#flask-py-docker-2              latest              a8fdbfef3095   23 hours ago    906MB

Once I ran the docker run with above image on particular port it got started in my local.

##docker run -d -p 5000:5000 flask-py-docker-2

and my simple hello world website is up and running. see png attachment

<img width="716" alt="image" src="https://user-images.githubusercontent.com/98540570/158225548-a8f1933c-92a3-479e-9c5a-4602324fb2ec.png">



Once it website is published we have to tag the docker image and push it to the ECR, using below commands.

docker tag flask-py-docker-2  527805459418.dkr.ecr.ap-northeast-1.amazonaws.com/flask-v1:latest

push command

docker push 527805459418.dkr.ecr.ap-northeast-1.amazonaws.com/flask-v1:latest


this will push the docker image to ECR.

Thanks YOu.
Looking forward to hear.

