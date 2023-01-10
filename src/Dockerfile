FROM python:3.7.3-stretch

RUN apt install git
RUN mkdir Normostrany
RUN git clone https://github.com/SimonaK11/Normostrany.git Normostrany
WORKDIR Normostrany
RUN pip install -r requirements.txt
# RUN pip install virtualenvwrapper
RUN python manage.py migrate
EXPOSE 80/tcp


CMD ["python", "manage.py", "runserver", "0.0.0.0:80"]