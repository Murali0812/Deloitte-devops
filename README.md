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




```
