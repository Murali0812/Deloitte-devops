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
    docker ps
   52  docker attach c5
   53  docker ps
   54  docker ps -a
   55  docker start c5
   56  docker ps
   57  docker exec -it c5 /bin/bash
   58  clear
   59  docker ps
   60  docker ps -a
   61  docker create -dt --name c6 centos:7
   62  docker create -t --name c6 centos:7
   63  docker ps
   64  docker ps -a
   65  clear
   66  docker ps -a
   67  docker stop c5
   68  docker ps -a
   69  docker rm -f c6
   70  docker ps -a
   71  docker run -it --name c7 ubuntu
   72  docker ps -a

docker run -dit --name c1 ubuntu
  108  docker ps
  109  docker run -dit --name c2 --hostname ramancontainer ubuntu
  110  docker ps
  111  docker exec -it c2 /bin/bash
  112  docker ps
  113  docker inspect c1
  114  ip a
  115  docker inspect c2
  116  clear
  117  docker ps
  118  docker rm -f `docker ps -aq`
  119  clear
  120  docker run -dit --name httpd httpd
  121  docker ps
  122  docker inspect httpd
  123  curl 172.17.0.2
  124  curl 172.17.0.2:80
  125  curl 172.31.23.145
  126  docker ps
  127  docker run -dit --name c2 -p 81:80 httpd
  128  docker ps
  129  docker inspect c2
  130  curl 172.31.23.145
  131  curl 172.31.23.145:81


```
