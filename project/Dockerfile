FROM python:3.8-slim

WORKDIR /app

COPY requirements.txt /app/

RUN pip install --no-cache-dir -r requirements.txt

COPY . /app/

EXPOSE 80

ENV FASTAPI_ENV=production

ENV DATABASE_URL="sqlite:///./sqlitedb/sqlitedata.db"

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]
