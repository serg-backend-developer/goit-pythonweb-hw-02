FROM python:3.12-alpine3.20

RUN apk add --no-cache build-base libpq-dev libpq

WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .

EXPOSE 8000

CMD ["python", "main.py"]
