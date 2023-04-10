# Deloitte-devops

```

ami :
ubuntu : Ubuntu Server 20.04 LTS (HVM), SSD Volume Type


inst type : t2.micro


created a keypair


-- instance created 

terminal :

moba xterm
cmd
gitbash
powershell


try to connect to instance with ssh-client

hostnamectl set-hostname docker


----

docker installation :

apt-get update -y

https://docs.docker.com/engine/install/ubuntu/


history :

 clear
    2  apt-get update -y
    3  clear
    4  sudo apt-get update
    5  sudo apt-get install     ca-certificates     curl     gnupg
    6  sudo mkdir -m 0755 -p /etc/apt/keyrings
    7  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
    8  echo   "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" |   sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    9  sudo apt-get update
   10  sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   11  docker -v
   12  systemctl status docker
   13  docker -v
   14  history




----
 docker ps
   19  docker ps -a
   20  ps -ef | grep docker
   21  docker -h
   22  clear
   23  docker images
   24  docker run -dt httpd
   25  docker ps
   26  docker images
   27  docker run -h
   28  docker run --help
   29  clear
   30  docker run -it httpd
   31  clear
   32  docker run -it --name c1 centos:7
   33  docker ps
   34  docker ps -a
   35  docker restart c1
   36  docker ps
   37  docker run -dit --name c2 centos:7
   38  docker ps
   39  docker run -dt --name c3 centos:7
   40  docker ps
   41  docker attach c3
   42  docker ps
   43  docker run -d --name c4 centos:7
   44  docker ps
   45  docker ps -a
   46  docker start c4
   47  docker ps
   48  docker run -d --name c5 httpd
   49  docker ps
   50  history




```
