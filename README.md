[![CircleCI](https://dl.circleci.com/status-badge/img/gh/sechibueze/udacity-alx-project-4-operationalize-ml/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sechibueze/udacity-alx-project-4-operationalize-ml/tree/master)

## Operationalize a Machine Learning Microservice-API

Deploy a containerized Python flask application to serve out predictions (inference) about housing prices through API calls. It uses a a pre-trained, sklearn model that has been trained to predict housing prices in Boston according to several features

## Project Procedure

- Test project code using linting
- Complete a Dockerfile to containerize this application
- Deploy containerized application using Docker and make a prediction
- Configure Kubernetes and create a Kubernetes cluster
- Deploy a container using Kubernetes and make a prediction
- Upload a complete Github repo with CircleCI to indicate the code has been tested

## Setup the Environment

- Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv.

```bash
python3 -m pip install --user virtualenv
# You should have Python 3.7 available in your host.
# Check the Python path using `which python3`
# Use a command similar to this one:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
```

- Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone: `python app.py`
2. Run in Docker: `./run_docker.sh`
3. Run in Kubernetes: `./run_kubernetes.sh`

### Kubernetes Steps

- Setup and Configure Docker locally
- Setup and Configure Kubernetes locally
- Create Flask app in Container
- Run via kubectl
