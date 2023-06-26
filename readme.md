# Basic Nginx Test

## About

The Basic Nginx Test repository provides a setup for running Azure DevOps agents in a Kubernetes cluster. It includes a simple test for Nginx deployments. The repository is primarily written in HTML.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine.

### Prerequisites

- Git
- Nginx
- Azure DevOps
- Kubernetes

### Installation

1. Clone the repo:
    ```bash
    git clone https://github.com/gokalpmeric/basicnginxtest.git
    ```

2. Navigate to the cloned directory:
    ```bash
    cd basicnginxtest
    ```

3. Deploy the application to your Kubernetes cluster. This will run Nginx as a pod. Use the following commands to apply the Kubernetes configurations:

    ```bash
    kubectl apply -f k8s-deployment.yaml
    kubectl apply -f k8s-service.yaml
    ```

## Repository Contents

The repository contains the following files:

- `azure-pipelines.yml`: This file contains the configuration for Azure Pipelines, which is used for setting up CI/CD.
- `index.html`: This is a basic HTML file used for testing the Nginx deployment.
- `k8s-deployment.yaml`: This file contains the configuration for a Kubernetes deployment, used to set up Azure DevOps agents.
- `k8s-service.yaml`: This file contains the configuration for a Kubernetes service, used to manage the Azure DevOps agents.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
