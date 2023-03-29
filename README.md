# Command to create a Docker Network
'docker network create docker_network'

# Command to run MySQL Docker Image
'docker run -d --name db --network docker_network -e MYSQL_ROOT_PASSWORD=my-secret-password mysql:latest'

# Running PhpMyAdmin Docker Image on the created network
'docker run -d --name phpmyadmin --network my_network -p 8080:80 phpmyadmin/phpmyadmin'
