# SCA-Cloud-School-Application
SCA Cloud School technical assessment

This is a django app in a docker container.

Run this app using the command:
`docker-compose up --detach`

## STEPS TO TEST THE APP
 ### This app is tested to ensure that it shows the HTTP 200 OK success status response code which indicates that the request has succeeded.

1. Run `docker ps` to get the details of the running container such as the id, image name, and port number.

2. Run `Invoke-WebRequest -Uri yourport` 
   in my case `Invoke-WebRequest -Uri http://localhost:8000/`
   It outputs something like this:
  ```
   StatusCode        : 200
   StatusDescription : OK
   Content           : <h1>Welcome to SCA Cloud School Application</h1>
   RawContent        : HTTP/1.1 200 OK
                       X-Frame-Options: SAMEORIGIN
                       Content-Length: 48
                       Content-Type: text/html; charset=utf-8
                       Date: Wed, 13 Jan 2021 05:41:09 GMT
                       Server: WSGIServer/0.2 CPython/3.9.1

                       <h1>Welcome to SC...
   Forms             : {}
   Headers           : {[X-Frame-Options, SAMEORIGIN], [Content-Length, 48], [Content-Type, text/html; charset=utf-8],
                       [Date, Wed, 13 Jan 2021 05:41:09 GMT]...}
   Images            : {}
   InputFields       : {}
   Links             : {}
   ParsedHtml        : mshtml.HTMLDocumentClass
   RawContentLength  : 48
  ```

## DEPLOYMENT TO DOCKERHUB
Run `docker push yourusername/yourdockerimagename` in my case `docker push cumioyemike/sca_welcome_web`
* The link to the dockerhub repository is https://hub.docker.com/repository/docker/cumioyemike/sca_welcome_web
