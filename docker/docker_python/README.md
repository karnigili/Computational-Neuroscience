## HOW TO


### Install Docker and launch the docker Daemon
1. Install the Docker is via the docker Desktop app
2. Launch the Docker daemon by simply opening the application (and wait until the status in the menu bar shows that docker has finished launching).


### Download and build
1. Download the docker_python/ directory 
2. In bash terminal build the container by `docker build . -t netpyne`

### Run
1. add python files you deisred to run to /docker_python/
2. PAY ATTENTION: The docker container will not display images- THUS make sure to save them to /home/data . for example - `simConfig.analysis['plotRaster'] = {‘saveFig':'/home/data/raster.png'}`
1. In bash terminal run the container via  `docker run -it  -v /docker_python/:/home/data  netpyne:latest python3 /home/data/name_of_file.py`
4. TIP: always use absolute paths !

Here, we mount a local directory docker_python/ to a virtual volume in the docker and run a file from this dicrtory using python.
