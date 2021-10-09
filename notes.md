# Notes

> notes taken during the course

<!-- https://gitignore.io -->
<!-- https://github.com/github/gitignore -->

https://www.confluent.io/hub/debezium/debezium-connector-mysql

https://github.com/codeedu/fc2-kafka-connect

```sh
docker-compose ps
docker exec -it fc-kafka-connect_mysql_1 bash

mysql -uroot -p fullcycle
root
show tables;
CREATE TABLE categories (id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(255));
show tables;
desc categories;
INSERT INTO categories (name) values('Eletronics');
SELECT * FROM categories;
```

Upload `mysql.properties` connector file to Control Center connectors section.
New topis:
- mysql-server
- mysql-server.fullcycle.categories
- mysql-history

```sh
INSERT INTO categories (name) values('Eletronics');
```

Check the messages of `mysql-server.fullcycle.categories` topic
