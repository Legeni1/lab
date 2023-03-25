# syntax=docker/dockerfile:1
FROM python:3.6-alpine
WORKDIR /opt
RUN pip install flask==1.1.2
EXPOSE 8080
ENV ODOO_URL: https://www.odoo.com/
ENV PGADMIN_URL: https://www.pgadmin.org/
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0
ADD /opt/  ./app.py
ENTRYPOINT ["python", "app.py","-g","daemon off"]



