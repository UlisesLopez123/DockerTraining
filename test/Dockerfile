# Base image
FROM python:3.12-slim

# Set Workspace
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
ENV PORT=5000
EXPOSE 5000
CMD ["python", "app.py"]

# docker build -t my-flask-app .
