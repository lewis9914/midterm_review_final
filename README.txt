The Dockerfile of the image we want to build should launch an extended version of a Jupyter
container with Redis already installed.

The docker-compose.yml file launches a complete development environment, instantiating  three different containers: 
-An extended version of a Jupyter container with Redis already installed (as specified in the Dockerfile);
-A Redis server;
-Portainer, to manage the containers in an interactive browser environment.

The GitHub action runs the Dockefile, installing Redis on the jupyter container, exposing port 80 and uploading
the image to DockerHub.

The docker directory contains the Dockerfile.
The work directory contains the saved Jupyter notebooks.
The github/workflows directory contains the yml file of the Github action. 


