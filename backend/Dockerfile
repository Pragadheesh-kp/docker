# Use an official Python runtime as the base image
FROM python:3.10-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container
COPY . /app

# Install the Python dependencies
RUN pip install --no-cache-dir flask flask-cors psycopg2-binary

# Expose port 5000 for the Flask application
EXPOSE 5000

# Define environment variables (update as needed)
ENV DB_NAME=cruddb
ENV DB_USER=postgres
ENV DB_PASSWORD=crudpass
ENV DB_HOST=3.110.153.93

# Command to run the backend application
CMD ["python3", "backend.py"]
