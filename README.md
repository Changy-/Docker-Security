Installation instructions for Docker:

  1. git clone https://github.com/Changy-/Docker-Security.git

  2. cd Docker-Security

  3. sudo make build

  4. sudo make binary

For example, once Docker is installed you can run a container which uses our security configuraion with the following command:
sudo docker run -it --security-opt seccomp=team_chupacabra_security.json ubuntu sh

Once inside the container you need to find a way to break the security configuration which blocks the risky system calls inside team_chupacabra_security.json.

Suggestion: Compile and run your own code inside of the container.

  1. Run apt-get update and install gcc, java jdk etc.
    apt-get update
    apt-get install gcc
    apt-get install default-jdk
    
  2. Install any text editor, for example vim
    apt-get install vim
 
