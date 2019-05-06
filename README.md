# docker
https://docker-curriculum.com/
https://docker-curriculum.com/#setting-up-your-computer
https://hub.docker.com/_/busybox/


NOTES:

IMAGE ID
html-server-image   v1                  edd69ecb7d76        47 hours ago        16.1MB
<none>              <none>              87ba89348424        2 days ago          16.1MB
nginx               alpine              0be75340bd9b        2 weeks ago         16.1MB
friendlyhello       latest              de9e9a4f2724        5 weeks ago         131MB
python              2.7-slim            8559620b5b0d        2 months ago        120MB


docker image rm  edd69ecb7d76;
docker image rm 87ba89348424;
docker image rm 0be75340bd9b;
docker image rm de9e9a4f2724;
docker image rm 8559620b5b0d;

docker image rm edd69ecb7d76 
Error response from daemon: conflict: unable to delete edd69ecb7d76 (must be forced) - image is being used by stopped container e6ff62ee06a9

 docker rmi -f <image_id> 
docker rmi -f edd69ecb7d76


#youtube
https://www.youtube.com/watch?v=YFl2mCHdv24
