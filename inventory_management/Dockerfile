# Dockerfile for inventory_management microservice
FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

ENV DATABASE_URL = "postgresql://sit722_task4_km4b_user:KB31SkKANSigdNw8gJmGFDl0hSBdrPPp@dpg-crp83tlds78s73d5qa1g-a.oregon-postgres.render.com/sit722_task4_km4b"

EXPOSE 7000

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "7000"]