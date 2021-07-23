# DockerTest

### Description of all files:

- Dockerfile      	- file for "docker build".
- app.py          	- MiniWebServer with ports 8080 on flask.
- requirements.txt	- The list of python requirements.
- resources       	- The folder where the content comes from to fill the web-page.
- docker-compose.yaml	- File which discribe process of run container
 
---------------------------------

### For build image and start container you need:
1. The first what you need its get the files from repo
 `git clone https://github.com/Lackronik/DockerTest.git`
(for the next updates use git pull from DockerTest directory)
2. Run `docker-compose up -d` from project directory


So now you can knock on your docker server address on port 8080.
You can change the text on site by edit <absolute path to directory>/DockerTest/web_app/resources/response.json
Edit the file, save, and then update the page.

For stop container use:
1. docker ps -qa (To check id of container)
2. docker stop <id of container>
