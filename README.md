# Catalogus Professorum Model
This project provides the data model for the Leipzig Professors Catalog
## Model
The model describes the vocabulary of the database.
* [Dokumentation](http://catalogus-professorum.org/cpm/2/)
## Tools
Tools so far are two docker containers. One is an Apache webserver that is used to provide the vocabulary documentation that is generated by the Tool Widoco (second docker container). Currently I could not solve the isue of using "more +6" in starup.sh. To teplay please use the following steps after docker-compose up:

```
docker exec -it tools_cpm-widoco_1 /bin/bash
/var/www# ./generate.sh 1
/var/www# ./generate.sh 1
```
