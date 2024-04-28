FROM python:3.8-buster
MAINTAINER Moucharaf (moucharafamadou0@gmail.com)
RUN apt-get update 
RUN apt update -y && apt install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
WORKDIR /
COPY requirements.txt  student_age.py /
RUN pip3 install -r /requirements.txt
VOLUME /data
EXPOSE 5000
CMD ["python", "./student_age.py"]
