# Use of the latest Ubuntu image from Docker
FROM ubuntu:latest

# Update the package list
RUN apt-get update -y

# Upgrade currently installed software
RUN apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Install Flask using pip3
RUN pip3 install flask

# Set the working directory in the container
WORKDIR /app/

# Copy the Python file to the container
COPY ./task2/api.py /app/api.py

# Expose port 5252 for the Flask app
EXPOSE 5252

# Run the Flask app
CMD ["python3", "api.py"]
