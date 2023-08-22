# Derived from official mysql image (our base image)
# Use mysql 5.7 as the flask-app is not set up to work with later versions

# Add a database and root password
# For hints on how to do this, consult the mysql 5.7 image documentation

# Add the content of the .sql file to your image
# All scripts copied to docker-entrypoint-initdb.d/ are automatically
# executed during container startup



FROM python:3.6

COPY . .

RUN pip install -r requirements.txt

ENV YOUR_NAME=James

EXPOSE 5050

ENTRYPOINT python3 app.py

