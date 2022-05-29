# Docker deployment on EC2 instance using Terraform

This is a simple project for the University, using Docker, docker-compose, AWS, Terraform & Bash

## Installation

### Creating the EC2 instance

```bash
cd aws
terraform init
terraform plan
terraform apply
```

### Creating the Docker image

```bash
cd docker
docker build . -t <USERNAME>/<IMAGE-NAME>:<TAG>
```

### Running docker-compose

To start the image:
```bash
docker-compose up
```

To stop the image:
```bash
docker-compose down
```
