
## HOW TO 

### Install Docker and launch the docker Daemon
1. Install the Docker is via the docker Desktop app
2. Launch the Docker daemon by simply opening the application (and wait until the status in the menu bar shows that docker has finished launching).


### Download and build
1. Download the docker_jupyter/ directory 
2. In bash terminal build the container by `docker build -t neuron_jupyter:latest .`

### Run
1. In bash terminal run the container via `docker run -it -p 8888:8888 neuron_jupyter:latest`
2. Enter the address shown in terminal (with the token) and work on jupyter via the browser
3. PAY ATTENTION- Filw won't save once docker is shut. download your important files.

