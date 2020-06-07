
docker info
-- 
show current docker instance information  

docker login
--
login to docker hub  

docker pull alpine
--
pull linux image   

docker images
--
list all images available in your account  

docker tag <image_id_3_unique_prefix> <tag_name>
--
tag an image   
image_id_unique_prefix - first 3+ unique portion of the image id  
tag_name - name of tag version ex: uresh09adl/alpine:tag_name1 || <username>/<name>:<tagged_name>  

docker pull uresh09adl/uresh88:testTag1
--
pull docker image from private repo  

docker image rm <image_id_3_unique_prefix> 
--
delete repo from local reposotory  
options --> -f to force delete  


* What is an example of a public registry? --Docker Hub
  


Docker Swan
--
used for docker occestration see image DockerSwan.png  
if node in swan cluster failed other applications will go to another worker node defined in swan cluster  
*How do you join a new manager node to a swarm cluster? --Use the swarm join command with the manager token.

*Users should be assigned roles and places into what Teams.

docker swarm init  
docker swarm join --token SWMTKN-1-5ewuic45cmgh4psvjeqfy5vhdttvznwtlu7tg9my6oip1yp1zu-8y2rf7vrc35kgrbqwble2nled 192.168.65.3:2377  

Back up Docker
--
-Docker swan cluster  
  stop docker --> systemctl stop docker
  cd var/lib/docker
  Copy and archive swarn directory
  start docker --> systemsctl start docker
  
-UCP  
  available command in docker copy and paste it

-Docker Trusted Registry (DTR)  
  back up content data -- docker provide us a command
  back up DTR meta data -- docker provide us a command
-Container volume data  
  should not be inside your containers -- best practise
  keep in a container volume
  container volume could save locally on Docker nodes, on a share that goes to NAS or SAN or even in public cloud
  

Docker Trusted Registry
--
Docker enprise edition has  
* docker engine
* docker UCP
* docker DTR

  * How do you deploy Docker Trusted Registry? --Deploy it as a container.

