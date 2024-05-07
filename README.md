# Sunbird-VA-Bot-Service



## Prerequisites
- Docker daemon must be running on your machine.
- Before running the project, ensure that you have an OpenAI key added to .env

## Setup Instructions

1. **Run Docker Daemon:**
   Ensure that Docker daemon is running on your machine.

2. **Start Redis Container:**
   Execute the following command to start the Redis container:
   ```
   docker run -d --name redis -p 6379:6379 -p 8001:8001 redis/redis-stack:latest
   ```

3. **Install Requirements:**
   Install the required Python dependencies by running:
   ```
   pip install -r requirements.txt
   ```

4. **Run the project:**
   Run the project using Uvicorn:
   ```
   uvicorn main:app --reload
   ```


To evaluate the performance improvement achieved by using Redis Semantic Cache, follow these steps:

1. **Run Test Script:**
   Execute the Python test script using the following command:
   ```
   python test.py
   ```

   This script will demonstrate the time saved by utilizing Redis Semantic Cache .


