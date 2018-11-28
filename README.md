# CaseWare JupyterLab

This repository contains everything you need to build a JupyterLab Docker image. It comes set up with some of the Machine Learning tools used by CaseWare's Research Team.

## Getting Started

These instructions will tell you how to build a Docker image for this project and run it as a container.


### Prerequisites

 - Docker, latest CE stable version. Executable file can be obtained at: https://store.docker.com/editions/community/docker-ce-desktop-windows

### Building

To build the Docker image, run the following command in the root directory of this repository: 
- `docker build -t jupyterlab-docker .`

This command will instruct Docker to build the image.

## Running

Once the image is built, run the following command to launch the container: 
- `docker run -p 8888:8888 jupyterlab-docker `

The container is now running and a number of messages will be printed to the terminal. This will include a security
token required to access JupyterLab in your browser. An example of the security token is provided, though yours will 
look slightly different: `http://(127.0.0.1):8888/?token=ed7a8cdaa38838e31f7d4a03145c97fa8ea88f92b4bc35a3`.

To access JupyterLab, simply point your host web browser to `localhost:8888/TOKEN`, where `TOKEN` is `/?token=ed7a8cdaa38838e31f7d4a03145c97fa8ea88f92b4bc35a3` in our example.

## Environment

 - `PYTHONPATH` - sets the search path for importing Python modules.
 - `IPYTHONDIR` - specifies which IPython is to be used.
 - `PYTHONUNBUFFERED` - tells Python that stdout and stdderr are to be unbuffered.

## Useful Links
 - More information about JupyterLab - https://jupyterlab.readthedocs.io/en/stable/index.html


