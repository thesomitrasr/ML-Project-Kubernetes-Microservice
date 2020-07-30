![CircleCI](https://img.shields.io/circleci/build/gh/somitrasr/ML-Project-Kubernetes-Microservice)

## Project Overview

In this project, we will apply the Machine Learning Microservice API skills. 

This udacity project containerizes a machine learning Python flask app using Docker and deploys it on a Kubernetes cluster.
The app mainly predicts housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. The data was initially taken from this site [Kaggle](https://www.kaggle.com/c/boston-housing).

---

### Project Tasks

The project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:
* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested
---

## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl


### Making predictions
In a separate terminal, run: `./make_prediction.sh`

---

### Project Structure
The project includes 4 directories:
- `model_data`, containing the machine learning models
- `output_txt_files`, containing the output of running a prediction on Docker and on Kubernetes
- `.circleci`, containing the configuration file to implement CI/CD through CircleCI
- `.git`, containing the git files


It also includes the following files:
- `app.py`, the main Python flask app
- `Dockerfile`, to define a Docker container
- `Makefile`, to build the project
- `make_prediction.sh`, to run predictions
- `README.md`, this file
- `requirements.txt`, containing the dependencies that are installed through the Makefile
- `run_docker.sh`, to launch a Docker container
- `run_kubernetes.sh`, to deploy containers on a Kubernetes cluster
- `upload_docker.sh`, to upload a Docker image to Docker Hub

---

## Authors
 - SomitraSR - [somitrasr](https://github.com/somitrasr)

