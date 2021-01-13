# SCA-Cloud-School-Application
SCA Cloud School technical assessment

This is a django app in a docker container.

Run this app using the command:
`docker-compose up --detach`

## STEPS TO TEST THE APP

1. Run `docker ps` to get the details of the running container such as the id, image name, and port number.

2. Run `Invoke-WebRequest -Uri yourport` 
   in my case `Invoke-WebRequest -Uri http://localhost:8000/`
   It outputs something like this:
   ![Alt Text](C:\Users\LENOVO\Picture\two.png)
