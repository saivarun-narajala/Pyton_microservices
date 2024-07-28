# Python Microservices Project

This project provides a tutorial on building a microservices architecture using Python. It includes services for user management, product management, and order processing.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Services](#running-the-services)
- [Project Structure](#project-structure)

## Prerequisites
Before you begin, ensure you have the following installed on your local machine:
- Python 3.8 or higher
- Docker
- Docker Compose
- Git

## Installation

### Step 1: Clone the Repository
    Clone this repository to your local machine using the following command:
    
      git clone https://github.com/scalablescripts/python-microservices.git
      cd python-microservices

### Step 2 : Set Up Virtual Environment

      # Create a virtual environment
      python -m venv venv
      
      # Activate the virtual environment
      # On Windows
      venv\Scripts\activate
      # On macOS/Linux
      source venv/bin/activate

### Step 3: Install Dependencies

Install the required Python packages using pip:


    pip install -r requirements.txt


## Running Services

### Step 4 : Start the Docker Containers


The project uses Docker to manage and run the microservices. Use Docker Compose to start all the services defined in the docker-compose.yml file:



    docker-compose up --build


### Step 5: Check Running Services


After running the above command, the microservices will be running on different ports. You can check the status and logs of the running services using:

    
    docker-compose ps
    docker-compose logs -f



## Project Structure

Here’s a brief overview of the project structure:


                python-microservices/
                │
                ├── user_service/
                │   ├── app.py
                │   ├── Dockerfile
                │   └── ...
                │
                ├── product_service/
                │   ├── app.py
                │   ├── Dockerfile
                │   └── ...
                │
                ├── order_service/
                │   ├── app.py
                │   ├── Dockerfile
                │   └── ...
                │
                ├── docker-compose.yml
                ├── requirements.txt
                └── README.md
