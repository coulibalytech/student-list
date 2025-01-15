# Download official Ubuntu 18.04
FROM python:3.8-buster

# Maintainer info & Description of dockerfile
LABEL maintainer="coulibalytech <cheick.coulibaly.pro@gmail.com>"
LABEL description="The dockerfile to build API Image with python:3.8-buster"


#Copy code source to working directory
COPY student_age.py /



# Install Prerequis package
RUN apt update -y && apt install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y

#Copy requirement file
COPY requirements.txt /
RUN pip3 install -r /requirements.txt


# Create a directory in the container
#RUN mkdir -p /data
# Declare the directory as a volume
#VOLUME /data
#Copy list student file in directory data
#COPY student_age.json /data

#DECLARE APÏ PORT
EXPOSE 5000

CMD ["python3", "./student_age.py"]


