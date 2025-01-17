FROM python:3.11-slim

WORKDIR /app

# Copy the requirements file
COPY requirements.txt .

# Install dependencies globally
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application code
COPY . .

# Make the run script executable
RUN chmod +x run.sh

# Expose the port your app will run on
EXPOSE 8001

# Run the app using the run script
CMD ["./run.sh"]


