Apache2 Server for PHP Projects
===============

Uses as base image [reinblau/debian](https://registry.hub.docker.com/u/reinblau/debian/)
and volume container add
-v  : /var/www


ex)
1.
sudo docker run -i -t -p 80:80 -v /home/henen/mysite/:/var/www -v /home/henen/apachelog/:/var/log/apache2 -d henen/apache2-php --link "DbcontainerName":db --name a2p5 /bin/bash 

2.
sudo docker exec "container name" service apache2 start



Installed Tools
---------------
* [Apache2](http://httpd.apache.org/)
* [PHP](http://php.net/)
