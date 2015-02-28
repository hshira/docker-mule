docker-mule
===================
Base docker image to run a Mule application server


Image tags
----------
```
    hshira/mule:latest
    hshira/mule:3.6
    hshira/mule:3.5
```


Usage
-----

To create the image `hshira/mule`, execute the following command on the docker-mule folder:

    docker build -t hshira/mule .

To run the image and bind to port :

    docker run -d --name docker-mule -p 8081:8081 hshira/mule

To ssh in the image

	docker exec -it docker-mule bash


All Set !
