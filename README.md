# GymGameBot
A repo that lets OpenAI Gym to build game bots to play games

## How to contribute codes

1. Always fetch the remote repo before committing

2. Use a unique branch to store your codes (create branch in github)

3. If there are no conflicts between the dev branch and the main branch
, then you can merge it to the main branch

## How to code in the repo

### 0. why so complicated

We use requirements.txt to make sure we are using packages of the same version, just like packages.json in javaScript, which manages project-specific dependencies and avoids potential conflicts.

We also use a "virtual environment" in this project, which is what the "venv" command creates for us. This ensures that your project's dependencies are isolated from your system-wide Python installation and other projects.

Note that this _env is the environment to run Python, not the OpenAI ".env" file.

### 1. create a virtual Python environment

template code

    python -m venv _env # _env is a suggested name
    python3 -m venv _env # if the previous one did not work

    source _env/bin/activate  # Linux/macOS
    _env\Scripts\activate      # Windows

    # then you are in the virtual environment!


### 2. install, update the packages using the requirements.txt

When you see

    (_env) username@device dir %

then you are in the virtual environment, and everything you do only modifies the virtual environment (_env) you created

Every time the requirements.txt becomes different
we can use install packages using this command.

When important packages are added to the environment, update the txt to let the team synchronized.

template code

    # install using the txt
    pip install -r requirements.txt

    # update the dependencies according to the requirements.txt
    pip install --upgrade -r requirements.txt

    # update the requirements.txt
    we actually need to manually update it...
    

