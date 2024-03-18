# ddp_prefect_starter

- Setup a virtual environment using ``` python3 -m venv <name> ```
- Activate the virtual env ``` source <name>/bin/activate ```
- Install the dependencies from requirements.txt ``` pip3 install -r requirements.txt ```
- If you are using any new packages, install them in your virtual env and use this to update the requirements.txt ``` pip3 freeze > requirements.txt ```
- Start the prefect orion server ``` prefect orion start ```
- To execute your flow you need to run an agent in different terminal ``` prefect agent start -q default ```. This will run the default queue worker.
