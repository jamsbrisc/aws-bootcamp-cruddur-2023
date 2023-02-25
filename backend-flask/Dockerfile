FROM python:3.10-slim-buster

# Inside Container
# make a new folder inside container
WORKDIR /backend-flask

# Outside Container -> Inside Container
# this contains the libraries we want to install to run the app
COPY requirements.txt requirements.txt

# Inside Container
# Install the python libraries used for the app
RUN pip3 install -r requirements.txt

# Outside container -> Inside Container
# means everything in the current directory
# first period represents everything in /backend-flash outside the container
# second period represents everything in /backend-flash inside the container
COPY . .

# environment variable set for the environment  (env vars)
# these are set inside the container and will remain set when the container is running
ENV FLASK_ENV=development

EXPOSE ${PORT}

# command 
# python3 -m flask run --host=0.0.0.0 --port=4567
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]