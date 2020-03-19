# pj1-local-deploy
This repo is used for recording any useful information for the local deployment for project 1

# docker-glassfish
1. cd docker-glassfish
2. build the image: ```docker build . -t glassfish-local```
3. run the image:   
```docker run --env AS_ADMIN_PASSWORD=abcd1234 --env AS_ADMIN_ENABLE_SECURE=1 -p 4848:4848 8080:8080 -d glassfish-local```
4. check if the container is running: ```docker ps```, you should see the container you just created.
5. Open your browser and enter localhost:4848 then click enter.
6. The username is `admin` and password is `abcd1234`.