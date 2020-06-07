
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



  


Docker Swan
--
used for docker occestration see image DockerSwan.png  
if node in swan cluster failed other applications will go to another worker node defined in swan cluster  
** swan comes under UCP(Universal Control Plane). So need to have Docker licened version.  
