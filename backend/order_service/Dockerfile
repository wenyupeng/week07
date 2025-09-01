# week07/backend/order_service/Dockerfile

FROM python:3.10-slim-buster

WORKDIR /code

LABEL author="sit722"

COPY requirements.txt .

RUN pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir -r requirements.txt

COPY app /code/app

EXPOSE 8000

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]