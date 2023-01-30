# Kubernetes Deployment Project

This project demonstrates the use of a Jenkins CI/CD pipeline to deploy a project over a Kubernetes cluster, utilizing various DevOps tools such as Github, Ansible, and AWS EC2 compute instances.

## Prerequisites

- An AWS account: this will be used to spin up three EC2 servers (one each for Jenkins server, Ansible serve and K8s server)
- Jenkins server set up and running
- Kubernetes cluster set up and running
- AWS CLI configured on the Jenkins server
- GitHub repository for the project

## Getting Started

1. Clone the project repository

2. Spin up three EC2 instances in your AWS account

3. Create a Jenkins pipeline job that pulls the project repository and triggers a build on commits.

4. Use Ansible to provision and configure the AWS EC2 instances that will be used to host the Kubernetes cluster.

5. Use the Jenkins pipeline to build and push a Docker image of the project to a registry (e.g. Docker Hub).

6. Use the Jenkins pipeline to deploy the image to the Kubernetes cluster on the EC2 instances, utilizing a Kubernetes deployment file.

7. Set up a Jenkins job to continuously monitor the deployed application and trigger a rolling update if any changes are detected.

## Deployment

The project can be deployed on the kubernetes cluster by running the following command:

## Monitoring

The project can be monitored using Kubernetes Dashboard or Prometheus and Grafana.

## Conclusion

This project demonstrates the use of a Jenkins CI/CD pipeline to deploy a project over a Kubernetes cluster, utilizing various DevOps tools such as Github, Ansible, and AWS EC2 compute instances. By automating the build, test, and deployment process, the project ensures that changes are quickly and safely rolled out to production.
