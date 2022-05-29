# Docker deployment on EC2 instance using Terraform

This is a simple project for the University, using Docker, docker-compose, AWS, Terraform & Bash

## Installation

### Creating the EC2 instance

```bash
cd aws
terraform init  # to download all the needed resources used in the Terraform file
terraform plan  # to check if the file has errors & to see the components output without creating it
terraform apply # to create all the components
```

### Creating the Docker image

```bash
cd docker
docker build . -t <USERNAME>/<IMAGE-NAME>:<TAG>
```

### Running the container with the script

To start the image:
```bash
cd aws
./run.sh
```

### Running the container without the script

First we need to go inside the `aws` folder.

To start the image:
```bash
docker-compose up
```

To stop the image:
```bash
docker-compose down
```
