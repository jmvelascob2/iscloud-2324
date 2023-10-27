FROM python:3.8-slim-buster
WORKDIR /app
COPY app.py /app
COPY requirements.txt /app

# Establecer la variable de entorno MYSQL_ROOT_PASSWORD
ENV MYSQL_ROOT_PASSWORD=p@ssw0rd1

RUN pip3 install -r requirements.txt
EXPOSE 5000
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]
