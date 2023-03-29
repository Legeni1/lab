# syntax=docker/dockerfile:1
FROM python:3.6-alpine
WORKDIR /opt
RUN pip install flask==1.1.2
EXPOSE 8080
ENV ODOO_URL: https://www.odoo.com/ PGADMIN_URL: https://www.pgadmin.org/
#ENV FLASK_APP=app.py
#ENV FLASK_RUN_HOST=0
COPY . /opt/  
ENTRYPOINT ["/usr/local/bin/python", "app.py","-g","daemon off"]



