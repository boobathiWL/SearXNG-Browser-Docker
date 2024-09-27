# Use an official Python runtime as a parent image
FROM python:3

# Set the working directory in the container
WORKDIR /app

# Copy requirements.txt and install dependencies
COPY ../requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# Copy the Searx application code
COPY ../searx ./searx

# Make port 8000 available to the world outside this container
EXPOSE 8000

# Run the application using Python
CMD ["python", "searx/webapp.py"]
