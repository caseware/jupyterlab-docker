# CaseWare JupyterLab

This repository contains everything you need to build a JupyterLab Docker image. It comes set up with some of the Machine Learning tools used by CaseWare's Research Team.

## Running

### Launch with Docker Run

Run the following command to launch the container: 
- `docker run -v /path/to/your/host/notebooks:/app -p 8888:8888 jupyterlab-docker`

### Launch with Docker Compose
- `docker-compose up`

In either case, the container is now running and a number of messages will be printed to the terminal. This will include a security
token required to access JupyterLab in your browser. An example of the security token is provided, though yours will 
look slightly different: `http://(127.0.0.1):8888/?token=ed7a8cdaa38838e31f7d4a03145c97fa8ea88f92b4bc35a3`.

To access JupyterLab, simply point your host web browser to `localhost:8888/TOKEN`, where `TOKEN` is `/?token=ed7a8cdaa38838e31f7d4a03145c97fa8ea88f92b4bc35a3` in our example.

## Environment

 - `PYTHONPATH` - sets the search path for importing Python modules.
 - `IPYTHONDIR` - specifies which IPython is to be used.
 - `PYTHONUNBUFFERED` - tells Python that stdout and stdderr are to be unbuffered.

## Useful Links
 - More information about JupyterLab - https://jupyterlab.readthedocs.io/en/stable/index.html


