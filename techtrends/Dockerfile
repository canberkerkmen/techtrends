FROM python:3.8
LABEL maintainer="Canberk Erkmen"

COPY . /app
WORKDIR /app

#install requirements
RUN pip install -r requirements.txt

#create database
RUN python init_db.py

#expose port
EXPOSE 3111

#run application
CMD [ "python", "app.py" ]