FROM ubuntu

WORKDIR /app

COPY requirements.txt /app
COPY devops /app

RUN sudo apt-get update && \
    sudo apt-get install -y python3 python3-pip && \
    sudo pip install -r requirements.txt && \
    cd devops

ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]




