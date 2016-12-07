git clone https://github.com/Changy-/Docker-Security.git

cd Docker-Security

sudo make build

sudo make binary

sudo docker run -it --security-opt seccomp=team_chupacabra_security.json ubuntu sh

Compile and run your own code:
  1. Run apt-get update and install gcc, java jdk etc.
    apt-get update
    apt-get install gcc
    apt-get install default-jdk
    
  2. Install any text editor, for example vim
    apt-get install vim
 
 Try and create a program which will successfully use a blocked system call from team_chupacabra_security.json
