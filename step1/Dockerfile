# Use the official Python base image
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the application code into the container
COPY . /app

# Install required Python packages
RUN pip install --no-cache-dir flask

# Expose the application port
EXPOSE 5000

# Command to run the application
CMD ["python", "app.py"]
