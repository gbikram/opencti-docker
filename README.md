# Self Host OpenCTI

## Ubuntu Setup
```bash
# Install Docker
> sudo apt update && apt-get update

# Run commands from https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository

# Setup repo to build containers
> git clone https://github.com/gbikram/opencti-docker.git
> cd opencti-docker
> cp env.example .env && source .env

# Run OpenCTI on Docker
> docker compose up -d

# Wait for a few mins for the platform to initialize

# Check if ES Database is running
> curl http://0.0.0.0:9200

# Visit http://<SERVER_IP>:8080/opencti to access the OpenCTI Web UI
```
