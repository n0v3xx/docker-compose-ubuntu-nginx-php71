# docker-compose-ubuntu-nginx-php71
Docker Setup for a Web Developer Ubuntu 16.04 with NGINX (1.10.0), PHP (7.1.5), OPcache and Xdebug (2.5.1)

This container setup build on: https://github.com/n0v3xx/docker-ubuntu-nginx-php7

!!! Modify the last line in "docker/bin/setup.sh" if you want to run a deployment.

**Run**

    chmod +x ./docker/bin/setup.sh
    ./docker/bin/setup.sh
    
Visit http://localhost:8990/info.php or https://localhost:8991/info.php
    
**Connect to Container**

    # Root
    sudo docker exec -it base_web /bin/bash
    
    # User
    sudo docker exec -itu myName base_web /bin/bash
    
**Restart or Stop**

    # Restart
    sudo docker-compose -f ./docker/ubuntu/php71/docker-compose.yml restart
    
    # Stop
    sudo docker-compose -f ./docker/ubuntu/php71/docker-compose.yml stop
