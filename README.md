
# ice_breaker

A repository for learning LangChain by building a generative ai application.

This is a web applicaiton crawling Linkedin & Twitter data about a person an customize an ice breaker with them. 

![udemy](https://img.shields.io/badge/LangChain%20Udemy%20Course-Coupon%20%2412.99-brightgreen)

## Before you begin - Pipenv

This project assumes that you have **Pipenv** installed.  Pipenv is a package management tool for Python that combines the functionality of pip (the Python package manager) and virtualenv (a tool for creating isolated Python environments). It is designed to simplify and streamline the management of Python packages and their dependencies within projects. Pipenv provides the following key features:

1. **Dependency Management**: Pipenv manages project dependencies by tracking them in a dedicated Pipfile. It records both the main packages required for your project and their specific versions.

1. **Automatic Virtual Environments**: When you create a new project or install dependencies using Pipenv, it automatically creates a virtual environment for that project. This ensures that project dependencies do not interfere with each other or with the system-wide Python installation.

1. **Dependency Resolution**: Pipenv uses a tool called pipfile.lock to lock the exact versions of packages and their dependencies. This guarantees that every developer working on the project uses the same package versions, promoting consistency across different environments.

1. **Simplified Workflow**: Pipenv provides a simple and streamlined workflow for package management. It combines commands for creating virtual environments, installing packages, and managing dependencies into a single tool.

1. **Security**: Pipenv also helps with security by providing information about known security vulnerabilities in your project's dependencies.

To get started with Pipenv, you typically navigate to your project directory, run `pipenv instal`l to install the required packages, and use `pipenv shell` to activate the virtual environment for your project. This allows you to work within a clean and isolated Python environment specific to your project's requirements.

Pipenv has gained popularity in the Python development community due to its user-friendly approach to managing Python packages and environments. However, it's worth noting that there are other tools available for similar purposes, and the choice of package management tool may depend on your specific project and team preferences.

### Install Pipenv

To install Pipenv on your system, you typically use the Python package manager `pip`, as Pipenv itself is a Python package. Here are the general steps to install Pipenv:

1. **Open a Terminal or Command Prompt:** Depending on your operating system, open a terminal or command prompt window. Make sure you have Python and pip installed. You can check this by running `python --version` and `pip --version`. If you don't have Python and pip installed, you'll need to install them first.

2. **Install Pipenv:** Use the following command to install Pipenv:

   ```
   pip install pipenv
   ```

   This command will download and install Pipenv from the Python Package Index (PyPI).

3. **Verify Installation:** After the installation is complete, you can verify that Pipenv is installed correctly by running:

   ```
   pipenv --version
   ```

   This should display the installed Pipenv version.

That's it! You've now successfully installed Pipenv on your system. You can use Pipenv to manage Python packages and virtual environments in your projects. To create a new Python environment and install packages for a specific project, navigate to the project directory and use `pipenv install`. To activate the virtual environment, use `pipenv shell`. For more detailed usage and commands, you can refer to the official Pipenv documentation.


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`PYTHONPATH=/{YOUR_PATH_TO_PROJECT}/ice_breaker`

`OPENAI_API_KEY`

`PROXYCURL_API_KEY`

`SERPAPI_API_KEY`

`TWITTER_API_KEY`

`TWITTER_API_SECRET`

`TWITTER_ACCESS_TOKEN`

`TWITTER_ACCESS_SECRET`

## Run Locally

Clone the project

```bash
  git clone https://github.com/emarco177/ice_breaker.git
  git clone git@github.com:ponessa/ice_breaker.git
```

Go to the project directory

```bash
  cd ice_breaker
```

Install dependencies

```bash
  pipenv install
```

Start the flask server

```bash
  pipenv run app.py
```


## Running Tests

To run tests, run the following command

```bash
  pipenv run pytest .
```


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://www.udemy.com/course/langchain/?referralCode=D981B8213164A3EA91AC)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/eden-marco/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://www.udemy.com/user/eden-marco/)

