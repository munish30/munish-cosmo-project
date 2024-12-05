# CosmoCloud Project Assignment

This is the project assignment where the top level folder named cosmocloud-deploy consists of helm chart for implementing a complete application stack with 1 scale replica of each frontend, backend, and a redis database on a cluster of Kubernetes.

## Tools/Utilities
This project assumes some tools to be installed previously before proceeding any further. Like:
- Minikube
- Kubectl(not an hard requirement but necesssary for post-deployment verfications)
- Container Engine(Requirement for minikube)

## Installation

```bash
git clone https://github.com/munish30/munish-cosmo-project.git
cd munish-cosmo-project
helm install testapp cosmocloud-deploy
```
The "testapp" is the name of the release that is given in the assignment. It can be changed to create a release with any name.

## Verifying the installation

```bash
minikube service frontend-svc
```
It will create a tunnel between minikube and host machine. It will also open the frontend deployment in the browser with the endpoint assigned by tunnel.

## Screenshots
![Screenshot from 2024-12-05 18-17-02](https://github.com/user-attachments/assets/25448cad-ba1f-4b55-a772-dbb772214da3)
