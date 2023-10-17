# Use a base Python image
FROM python:3.9

# Set the working directory to /app
WORKDIR /app

# Copy the dependency requirements file
COPY requirements.txt .

# Install the dependencies using pip
RUN pip install --no-cache-dir -r requirements.txt

# Copy the entire project into the container's working directory
COPY . .

# Set the environment variable for Flask
ENV FLASK_APP=app.py

# Expose port 5000 for Flask
EXPOSE 5000

# Command to run the application when the container starts
CMD ["python", "app.py"]