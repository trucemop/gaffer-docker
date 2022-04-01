
```
docker-compose up
```

Access the HDFS NameNode web UI at: http://localhost:9870

Access the Accumulo Monitor UI at: http://localhost:9995

Access the NiFi UI at https://localhost:8443/nifi/

user and pw in .env SINGLE_USER_CREDENTIALS fields 

accumulo credentials in conf/client.conf principal token fields

can get shell with (use token field in client.conf for pw):
docker exec -it accumulo-master accumulo shell -u root
