# Use an official Python runtime as a base image
FROM python:3.8

# Set the working directory in the container
WORKDIR /appointments

# Copy the requirements file into the container at /app
COPY . /appointments/



# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir Flask==2.0.2



# # Copy the current directory contents into the container at /app
# COPY . /app

# Expose port 7070 to the outside world
EXPOSE 7070

# Define environment variable
ENV NAME appointments

# Run appointments.py when the container launches
CMD ["python", "appointments.py"]
