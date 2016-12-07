###Installation instructions for Docker:
```
  git clone https://github.com/Changy-/Docker-Security.git

  cd Docker-Security

  sudo make build

  sudo make binary
```

Alternatively, you can install docker using: ```sudo apt-get install docker``` and copying https://github.com/Changy-/Docker-Security/blob/master/team_chupacabra_security.json into your working directory.

For example, once Docker is installed you can run a container which uses our security configuraion with the following command:
```
sudo docker run -it --security-opt seccomp=team_chupacabra_security.json ubuntu sh
```
Once inside the container you need to find a way to break the security configuration which blocks the risky system calls inside team_chupacabra_security.json.

###Compile and run your own code inside of the container.
```
  1. Run apt-get update and install gcc, java jdk etc.
    apt-get update
    apt-get install gcc
    apt-get install default-jdk
    
  2. Install any text editor, for example vim
    apt-get install vim
``` 
