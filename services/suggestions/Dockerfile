# Use the official Python image
FROM python:3.11-slim

# Set working directory
WORKDIR /app

# Install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy app files
COPY . .

# Expose the port uvicorn will run on
EXPOSE 4444

# Run the app
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "4444"]
