# ddp_prefect_starter For DostEducation analytics

This DDP prefect starter us being used to setup DostEducation's Prefect based infrastructure setup.

## Installation

### Prerequisite
1. pyenv - for maintaining multiple python versions
2. python 3.8.10

### Steps
1. Clone the repository
    ```sh
    git clone https://github.com/DostEducation/prefect_deployments.git
    ```
2. Switch to project folder and setup the virtual environment
    ```sh
    cd prefect_deployments
    python3 -m venv venv
    ```
3. Activate the virtual environment
    ```sh
    source ./venv/bin/activate
    ```
4. Install the dependencies from requirements.txt:
    ```sh
    pip3 install -r requirements.txt
    ```
5. After any new packages introduced, install them in your virtual env and use this to update the requirements.txt:
    ```sh
    pip3 freeze > requirements.txt
    ```
6. Start prefect orion server
    ```sh
    prefect orion start
    ```
7. To execute your flow you need to run an agent in different terminal (This will run the default queue worker).
    ```sh
    prefect agent start -q default
    ```
