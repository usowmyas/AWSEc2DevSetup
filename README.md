# AWS EC2 Dev Setup
## Create a EC2 in AWS and ssh into it using key


## INSTALL Docker
```bash
sudo yum update
sudo yum install -y docker
```

## START give necessary permissions and start docker
```bash
sudo usermod -a -G docker ec2-user
sudo service docker start
```

## INSTALL docker-compose
```bash
sudo curl -L "https://github.com/docker/compose/releases/download/1.9.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

## give permissions to docker-compose
```bash
sudo chmod +x /usr/local/bin/docker-compose 
```

## Exit from ec2
```bash
exit
```

## Re-login , check docker & docker-compose versions
```bash
docker --version
docker-compose --version
```

