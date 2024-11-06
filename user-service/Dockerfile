# Use the Python 3.8 slim image as the base
FROM python:3.8-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file and install dependencies
COPY requirements.txt .
RUN pip install -r requirements.txt

# Copy the application code into the container
COPY . .

# Expose port 5000, which the service will use
EXPOSE 5000

# Command to start the service
CMD ["python", "app.py"]
