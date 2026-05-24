FROM python:3.11

WORKDIR /app

COPY . .

RUN pip install flask flask-cors

EXPOSE 5000

CMD ["python", "app.py"]