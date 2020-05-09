FROM python:2.7-stretch
MAINTAINER 306826@supinfo.com
ADD ./simple_api/student_age.py /
RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip install flask flask_httpauth flask_simpleldap python-dotenv
EXPOSE 5000
WORKDIR /
CMD [ "python", "./student_age.py" ]
