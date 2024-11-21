### If you are reading this, I have either forgotten to remove the text in time or worse, you are currently reviewing my paper and I have not yet updated this repository.

### Due to problems with the UKE's VPN access, this repository could not be finished in time for the deadline of my thesis, but it will be updated soon.

# Project template: Python without GPU 
This repository represents a blueprint for projects with Python:

- Python 3.9, git, and pip
- Linter for appropiate code standards (and config files for reasonable defaults)
    - flake8
    - pyLint
- Code formatter: black

## Usage
Specify the packages you require in the *requirements.txt*. More complex environment customization goes into *Dockerfile*.

While using Visual Studio Code for development is encouraged, the image does not depend on this IDE in any way. As a side effect, its required server components are not even installed by default if the Dockerfile in root is built manually. Opening the project in VS Code will set the proper default and configure everything appropriately. Alternatively, build the container with `docker build -t <YOUR PROJECT NAME>:0.1 .` and run the container with `docker run -p <YOUR LOCAL PORT>:22 --rm --gpus all <YOUR PROJECT NAME>:0.1`.
