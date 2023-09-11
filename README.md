# CI/CD Data Science with Python

## Setup
* #Install Dependencies
make install

* #Lint with Rull
make lint

* #Format with Black
make format

## Files

* .devcontainer/ -- configures local development container environment
  
* .github/workflows/app.yml -- triggers CI/CD on automated build, test, and deployment pipelines

* "Makefile" -- configuration file used in Unix-based systems for automating tasks and building software. 

* "app.py" -- Python example file.

* "requirements.txt" is to specify the dependencies (libraries and packages) required to run the project.

## CI/CD

CI/CD flow is triggered by GitHub Actions, to run the Makefile are as follows: make install, make format, and make lint. 

1. Set up job
2. Run actions/checkout@v3
3. Setup python 3.x
4. Install dependencies
5. Lint with Ruff
6. Format with Black
7. Post set up Python 3.x
8. Post Run actions.checkout@v3
9. Complete job

## Status
You can find successful build jobs from Git Action (https://github.com/minlingz/706miniP1/actions/runs/6061466759). The workflow passed 5 versions of pythons, 3.7, 3.8, 3.9, 3.10, 3.11. Each build job contains subtasks as shown below.

![Alt text](p1build.png)
