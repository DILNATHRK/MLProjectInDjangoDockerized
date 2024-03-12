#   use an official pyhton runtime as a parent image 
FROM python:3.9

ENV PYTHONBUFFERED 1

# set working directory in the container
WORKDIR /app

# copy curent directory files into container at  /app
COPY . /app 

# install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# expose the port to 8000

EXPOSE 8000

# Define the command to run the application

CMD ["python","manage.py","runserver","0.0.0.0:8000"]