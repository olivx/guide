# Manual Docker LinuxTip

### instalação 
curl  -fsSL https://get.docker.com/ | sh

### primeira docker container 
sudo docker run hello-world

### visualizar o container en execução
sudo docker ps

### visualizar todos os containers 
sudo docker ps -a 

### visualizar as imagens 
sudo docker images 

##### -d para rodar em backgraund 
#### -ti para executar interratividade com terminal 
#### /bin/bash para que possa executar o terminal 
#### ubuntu é o nome da imagem a ser executada, caso não exista será feito o download do dockerhub
sudo docker run -ti ubuntu /bin/bash

### saindo do container 

ctrl+d mata o container e sai
ctrl+pq sai do container e deixa o mesmo em execução

### retrornado ao container 
sudo docker attach CONTAINER ID

### crear container mas não coloca em execução
sudo docker create ubuntu 

### para um container se estar no mesmo 
sudo docker stop CONTAINER ID

### iniciar o container 
sudo docker start CONTAINER ID

### pausar um container 
sudo docker pause CONTAINER ID 

### tirar da pausa 
sudo docker unpause CONTAINER ID 

### verificar os logs do container 
sudo docker logs CONTAINER ID 

### verficar os processo em execução 
sudo docker top CONTAINER ID 

### verificar os quanto esta consumindo de memoria e cpu 
sudo docker stats CONTAINER ID 

### remover um container -f caso o mesmo esteja em execução
sudo docker rm -f CONTAINER ID 

