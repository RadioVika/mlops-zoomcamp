Connecting to EC2 instance
`ssh -i ~/.ssh/mlops-zoomcamp.pem ubuntu@3.67.34.146`

Using short name
`~/.ssh/config`
```
Host mlops-zoomcamp
    HostName 3.70.208.174
    User ubuntu
    IdentityFile ~/.ssh/mlops-zoomcamp.pem
    StrictHostKeyChecking no
```
`ssh mlops-zoomcamp`

## Setup instance
`sudo apt update`

### Download Anaconda 
`https://repo.anaconda.com/archive/Anaconda3-2023.03-1-Linux-x86_64.sh`

### Install Docker
`sudo apt install docker.io`

### Install docker-compose
`mkdir soft`
`cd soft`

https://github.com/docker/compose - > Releases -> docker-compose-linux-x86_64
Download
`wget https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-x86_64 -O docker-compose`
Make it executable
`chmod +x docker-compose`

Make files in soft folder accesible
`nano .bashrc`
add line
`export PATH="${HOME}/soft:${PATH}"`
`source .bashrc`

Follow instructions
https://docs.docker.com/engine/install/linux-postinstall/


### Installing and running Jupyter Notebook
```bash
mkdir notebooks
cd notebooks
jupyter notebook

```