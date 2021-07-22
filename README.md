# DockerTest

### Description of all files:

Dockerfile	- file for "docker build".

app.py		- MiniWebServer with ports 8080 on flask.

requirements.txt- The list of python requirements.

resources	- The folder where the content comes from to fill the web-page.

---------------------------------
For build image you need:
1. The first what you need its get the files from repo
 `git clone https://github.com/Lackronik/DockerTest.git` (for the next updates use git pull from DockerTest directory)
2. Now need to build image, use: `docker build -t web-hello .` (from DockerTest directory)
3. Lets start container, use: `docker run --rm --name web -p 8080:8080 -v <absolute path to directory>/DockerTest/resources:/usr/src/app/resources -d web-hello`
4. For check correctness use: `docker ps`

So now you can knock on your docker server address on port 8080.
For stop container use:
1. docker ps -qa (To check id of container)
2. docker stop <id of container>
