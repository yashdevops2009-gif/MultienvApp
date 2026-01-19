# backend/dev/Dockerfile
FROM python:3.11-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
ENV FLASK_APP=app.py
ENV FLASK_RUN_PORT=3001
CMD ["flask", "run", "--host=0.0.0.0", "--port=3001"]
