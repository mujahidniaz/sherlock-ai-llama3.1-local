# Use the official Python image from the Docker Hub
FROM python
# Set the working directory
WORKDIR /app
RUN mkdir /data
# Copy the requirements file into the container
COPY requirements.txt requirements.txt

# Install the dependencies
RUN pip install -r requirements.txt

# Copy the rest of the application code into the container
COPY . .

# Expose port 8000
EXPOSE 8000

# Command to run the application
CMD ["python", "app.py"]