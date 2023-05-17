# TestFastApiAndDocker

This repository shows how to dockerize fast api application

steps to run

        docker build -t buildocker:0.5 .

        docker run -p 8000:8000 --name ton buildocker:0.5

To see current docker containers

        docker ps -a

To run the docker

        docker run -p 8000:8000 --name ton buildocker:0.5

To run docker by container id
    
        docker start -i  <container-id>
  
To run fast-api application standalone
        
        uvicorn app.main:app --reload
  
To  remove docker container
        
        docker rm <container-id>  
