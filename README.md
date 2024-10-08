# opentofu-docker-ubuntu

This script provides a Docker-based Ubuntu environment for running OpenTofu on M1 Macs and above. Due to potential compatibility issues with OpenTofu’s local planning on M1 Mac systems, this setup ensures smooth execution within a containerized Ubuntu environment.

This description keeps it concise and to the point, emphasizing the purpose of the script and the issue it addresses on M1 Macs.

## Usage

### Build the Docker Image
```
$ docker build --platform linux/amd64 -t opentofu-env .
```

### Set Up Alias for the Shell Script
```
$ vi ~/.zshrc
```
Add the following line:
```
alias tofuplan='/your/directory/opentofu.sh’
```
### Update Shell Configuration
```
$ source ~/.zshrc
```
### Run Plan
```
$ cd "/your/workdir"
$ tofuplan
```
