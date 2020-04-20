FROM python:2.7-alpine3.7
WORKDIR /app
COPY app.py requirements.txt ./
RUN ["pip", "install", "-r", "requirements.txt"]
ENV PYTHONPATH /app
ENV FLASK_APP app:flask_app
CMD ["run", "-h", "0.0.0.0", "-p", "80"]
ENTRYPOINT ["flask"]
