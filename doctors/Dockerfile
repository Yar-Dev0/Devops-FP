# Use an official Python runtime as a base image
FROM python:3.8

# Set the working directory in the container
WORKDIR /doctors

# Copy the requirements file into the container at /app
COPY . /doctors/

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir Flask==2.0.2

# Copy the current directory contents into the container at /app
# COPY . /doctors

# Expose port 9090 to the outside world
EXPOSE 9090

# Define environment variable
ENV NAME doctors

# Run doctors.py when the container launches
CMD ["python", "doctors.py"]
