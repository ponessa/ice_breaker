
# ice_breaker

A repository for learning LangChain by building a generative ai application.

This is a web applicaiton crawling Linkedin & Twitter data about a person an customize an ice breaker with them. 

![udemy](https://img.shields.io/badge/LangChain%20Udemy%20Course-Coupon%20%2412.99-brightgreen)

## Before you begin

**Pipenv**

This project assumes that you have **Pipenv** installed.  Pipenv is a package management tool for Python that combines the functionality of pip (the Python package manager) and virtualenv (a tool for creating isolated Python environments). It is designed to simplify and streamline the management of Python packages and their dependencies within projects. Pipenv provides the following key features:

1. **Dependency Management**: Pipenv manages project dependencies by tracking them in a dedicated Pipfile. It records both the main packages required for your project and their specific versions.

1. **Automatic Virtual Environments**: When you create a new project or install dependencies using Pipenv, it automatically creates a virtual environment for that project. This ensures that project dependencies do not interfere with each other or with the system-wide Python installation.

1. **Dependency Resolution**: Pipenv uses a tool called pipfile.lock to lock the exact versions of packages and their dependencies. This guarantees that every developer working on the project uses the same package versions, promoting consistency across different environments.

1. **Simplified Workflow**: Pipenv provides a simple and streamlined workflow for package management. It combines commands for creating virtual environments, installing packages, and managing dependencies into a single tool.

1. **Security**: Pipenv also helps with security by providing information about known security vulnerabilities in your project's dependencies.

To get started with Pipenv, you typically navigate to your project directory, run `pipenv instal`l to install the required packages, and use `pipenv shell` to activate the virtual environment for your project. This allows you to work within a clean and isolated Python environment specific to your project's requirements.

Pipenv has gained popularity in the Python development community due to its user-friendly approach to managing Python packages and environments. However, it's worth noting that there are other tools available for similar purposes, and the choice of package management tool may depend on your specific project and team preferences.

**Pyenv and asdf**

This project also requires either `pyenv` or `asdf`. `pyenv` and `asdf` are two popular version management tools for programming languages, primarily used for managing different versions of Python and other languages like Node.js, Ruby, and more. They help developers switch between different language versions and manage dependencies more efficiently. Here's a brief overview of each:

1. **pyenv:**

   - **Purpose:** `pyenv` is a version management tool specifically designed for Python. It allows you to install and switch between multiple Python versions on your system.
   
   - **Key Features:**
     - Installing and managing different Python versions side by side.
     - Setting a global Python version for your system or configuring specific versions on a per-project basis.
     - Automatically setting the appropriate Python version for a project based on a `.python-version` file or other configuration.
   
   - **Usage:** To use `pyenv`, you can install it on your system and then use commands like `pyenv install`, `pyenv global`, and `pyenv local` to manage Python versions. It's commonly used by Python developers to work with different Python versions, especially when compatibility issues arise.

2. **asdf (formerly known as asdf-vm):**

   - **Purpose:** `asdf` is a more general-purpose version manager that supports multiple languages, including Python, Node.js, Ruby, and more. It allows you to switch between different language runtimes and versions seamlessly.
   
   - **Key Features:**
     - Managing different versions of various programming languages.
     - Easily setting the version of a language on a per-project basis using `.tool-versions` files.
     - Plugin-based architecture that allows you to extend its functionality to support additional languages.
   
   - **Usage:** To use `asdf`, you install it and its language-specific plugins for the languages you work with. Then, you can switch between language versions using `asdf global`, `asdf local`, and other commands, much like `pyenv`. `asdf` is favored by developers who work with multiple programming languages and want a unified version management solution.

Both `pyenv` and `asdf` are valuable tools for developers who need to manage multiple versions of programming languages to ensure compatibility with different projects or libraries. The choice between them depends on your specific needs and whether you primarily work with Python or multiple languages.


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

### Install Pyenv

Installing `pyenv` on a Mac with an Apple M1 (Apple Silicon) chip requires a few additional steps due to the different architecture. Here are the steps to install `pyenv` on a Mac with an M1 chip:

1. **Install Homebrew:** If you don't have Homebrew installed, it's a package manager for macOS that makes it easier to manage software packages. You can install it by running the following command:

   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install Dependencies:** You'll need some dependencies to build Python versions with `pyenv`. Install them via Homebrew:

   ```bash
   brew install zlib sqlite bzip2
   ```

3. **Install `pyenv` with Homebrew:** Use Homebrew to install `pyenv`:

   ```bash
   brew install pyenv
   ```

4. **Add `pyenv` to Your Shell Profile:** Add the following lines to your shell profile file (e.g., `~/.zshrc` for Zsh or `~/.bashrc` for Bash):

   ```bash
   if command -v pyenv 1>/dev/null 2>&1; then
     eval "$(pyenv init -)"
   fi
   ```

   Save the file and then run the following command to apply the changes:

   ```bash
   source ~/.zshrc  # For Zsh users
   ```

   Or for Bash:

   ```bash
   source ~/.bashrc  # For Bash users
   ```

5. **Install Python Versions:** You can now use `pyenv` to install different Python versions, including versions that are compatible with the M1 chip. For example, to install Python 3.9.6:

   ```bash
   pyenv install 3.9.6
   ```

6. **Set Global Python Version:** You can set a global Python version for your system using `pyenv global`. For example:

   ```bash
   pyenv global 3.9.6
   ```

7. **Verify Installation:** To verify that `pyenv` and the installed Python versions are working correctly, you can run:

   ```bash
   pyenv versions
   ```

   This command should list the installed Python versions.

With these steps, you should have `pyenv` installed on your Mac with an Apple M1 chip, and you can use it to manage and switch between different Python versions for your projects.


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

