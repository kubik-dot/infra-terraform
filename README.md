# infra-terraform
================

## Description
------------

infra-terraform is an open-source, cloud-agnostic infrastructure as code (IaC) tool that leverages Terraform to provision and manage cloud resources. It provides a simple and consistent interface for defining and managing infrastructure across multiple cloud providers.

## Features
------------

* **Cloud-Agnostic**: Supports multiple cloud providers, including AWS, Azure, and Google Cloud Platform.
* **Infrastructure as Code (IaC)**: Define infrastructure using human-readable configuration files (HCL) and manage changes through version control.
* **Automated Provisioning**: Quickly provision infrastructure resources with Terraform's state management.
* **Configurable**: Customize infrastructure setup using variables and input values.
* **Extensive Documentation**: Complete documentation for Terraform configurations and best practices.

## Technologies Used
-------------------

* **Terraform**: Open-source IaC tool from HashiCorp
* **HCL**: Human-readable configuration language for Terraform
* **GitHub**: Source code management and repository hosting
* **Docker**: Containerization for repeatable and consistent builds
* **Makefile**: Automated build and deployment scripts

## Installation
------------

### Prerequisites

* Docker installed on your system
* Terraform installed on your system
* GitHub account for authentication

### Installation Steps

1. Clone the repository using `git clone https://github.com/your-username/infra-terraform.git`
2. `cd` into the cloned repository
3. Run `docker build -t infra-terraform .` to build the Docker image
4. Run `docker run -it --rm -v $(pwd):/workspace infra-terraform:latest` to start the Docker container
5. Apply Terraform configuration using `terraform init` and `terraform apply`

### Configuration

* Create a `terraform.tfvars` file in the root directory with your desired input values
* Update `main.tf` and `variables.tf` files as needed for your specific infrastructure setup

## Contributing
------------

We welcome contributions to the project! Please follow these guidelines:

* Fork the repository and create a new branch for your feature or bug fix
* Submit a pull request with a clear description of your changes
* Ensure thorough testing and documentation of your changes

## License
--------

This project is licensed under the MIT License. See the [LICENSE file](LICENSE) for details.

## Authors
---------

* Your Name
* [Your Email](your@email.com)
* [Your GitHub Profile](https://github.com/your-username)

## Acknowledgments
---------------

* HashiCorp for Terraform
* Docker for containerization
* GitHub for source code management