# Powershell

```
Set-ExecutionPolicy RemoteSigned
```

# Prompt lendário para node windows 

```
git clone https://github.com/jasongin/nvs
cd nvs
.\nvs install
notepad $PROFILE
Import-Module "$env:LOCALAPPDATA\nvs\nvs.psm1"
nvs --version
```

# Docker Portainer

```
docker pull portainer/portainer-ce

docker volume create portainer_data

docker run -d -p 9000:9000 -p 8000:8000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce
```

# RabbitMQ

```
docker run -d --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3-management
```
