#branch secure
* Unordered sub-list.
* Unordered sub-list-2.
***
### DOCKER

---

- create a docker network.

  #### Command: docker network create mysql

---

- command that will run a mysql:latest docker image with the name of db with a root password=my-secret-password.

  #### Command: docker run --network mysql -v $(pwd)/db/datadir:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=my-password --name mysql -d mysql

---

- Provide a command that will run the docker image phpmyadmin/phpmyadmin on the network previously created mapping a port of your choice to port 80 of the container

  #### Command: docker run --network mysql -p 83.212.126.240:8083:80 -e PMA_HOST=mysql -d phpmyadmin/phpmyadmin

---
