# CI/CD Tools and Practices Final Project

## Project Name

**ci-cd-final-project**

## Description

This repository contains the final project for the **CI/CD Tools and Practices** course. The project demonstrates the implementation of a **Continuous Integration (CI) pipeline** using GitHub Actions. The pipeline automates code checkout, dependency installation, linting, and unit testing to ensure code quality and reliability.

## CI Pipeline Features

The GitHub Actions workflow performs the following tasks:

* **Checkout Source Code** – Retrieves the project code from the repository.
* **Install Dependencies** – Installs Python dependencies using `pip`.
* **Linting with Flake8** – Checks the code for style issues, syntax errors, and complexity problems.
* **Unit Testing with Nose** – Executes automated unit tests and measures test coverage.

## Workflow Trigger

The CI workflow is triggered automatically when:

* Code is **pushed to the `main` branch**
* A **pull request is created targeting the `main` branch**

## Technologies Used

* **GitHub Actions** – CI pipeline automation
* **Python 3.9** – Application runtime
* **Flake8** – Code linting and quality checks
* **Nose** – Unit testing framework
* **Docker Container (`python:3.9-slim`)** – Workflow runtime environment

## Repository Structure

```
ci-cd-final-project
│
├── .github/
│   └── workflows/
│       └── workflow.yml
│
├── service/
├── tests/
├── requirements.txt
└── README.md
```

## Setup Instructions

1. Clone the repository:

```
git clone https://github.com/YOUR_USERNAME/ci-cd-final-project.git
```

2. Navigate to the project directory:

```
cd ci-cd-final-project
```

3. Install dependencies:

```
pip install -r requirements.txt
```

4. Run tests locally:

```
nosetests -v
```

## Author

**Mazen Naji**

## License

This project is licensed under the **Apache License**.

---

© IBM Corporation 2023. All rights reserved.
