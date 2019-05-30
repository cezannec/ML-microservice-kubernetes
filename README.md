[![CircleCI](https://circleci.com/gh/cezannec/ML-microservice-kubernetes.svg?style=svg)](https://circleci.com/gh/cezannec/ML-microservice-kubernetes)

## Repository Overview

This repository contains code to containerize a machine learning, Python application; it uses a pre-trained `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). 

`app.py` serves out predictions about housing prices through API calls. This code could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

Instructions for running the app using Docker or Kubernetes can be found below.

---

## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes-Specific Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create a Flask app in a Container
* Run via kubectl 
* You can choose to run one cluster locally with [Minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/)
