Monitoring Setup Guide

This README provides instructions for setting up monitoring using Grafana and Prometheus as part of the project 

infrastructure. These tools are essential for observing and analyzing the performance and health of the systems 

deployed, ensuring proactive management of resources and quick troubleshooting.

Prerequisites

Before proceeding, ensure you have the following installed on your system:

-Docker

-Docker Compose

These tools will help in deploying Grafana and Prometheus through Docker containers, making the setup process 

straightforward and reproducible.

Installation Steps

1. Clone the Project Repository

Start by cloning the project repository which contains the necessary Docker configurations:

git clone https://example.com/your-repo.git

cd your-repo/Monitoring

2. Setup Environment Variables

Modify the sample environment configuration files as needed:
# Adjust this file to set environment-specific variables
nano .env 

Make sure to configure the necessary details such as database connections or API keys.

3. Deploy with Docker Compose

Navigate to the monitoring directory and deploy the services:

docker-compose up -d

This command will start Prometheus and Grafana as defined in your docker-compose.yml.

4. Verify the Installation

Ensure the containers are running correctly:


docker-compose ps

You should see the Grafana and Prometheus services running.

5. Access Grafana Dashboard

Grafana is typically accessed via web browser:

http://localhost:3000   # Replace localhost with your server IP if necessary


Configuring Prometheus

Edit Config File: Adjust the Prometheus configuration to fine-tune your monitoring settings or add new targets.

Reload Configuration: Reload Prometheus configuration without restarting the service:

curl -X POST http://localhost:9090/-/reload  # Only if you have set up Prometheus to allow reloading via HTTP

Documentation

For more detailed information on configuring and using Grafana and Prometheus, refer to the official documentation:

-Grafana Documentation

-Prometheus Documentation