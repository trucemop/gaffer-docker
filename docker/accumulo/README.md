
```
docker-compose up
```

Access the HDFS NameNode web UI at: http://localhost:9870

Access the Accumulo Monitor UI at: http://localhost:9995

Access the NiFi UI at https://localhost:8443/nifi/

user and pw in .env SINGLE_USER_CREDENTIALS fields 

it will take awhile to build and start.  containers will show exit 1 for a bit while everything settles.
after accumulo is up, grant root pii auths with (password: secret):
docker exec -it accumulo-master accumulo shell -u root -e 'addauths -s pii -u root'
