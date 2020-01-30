1. Clone the following repository (if not already);
- https://github.com/theocrithary/Piper-2020/tree/master/Day%202/Docker
2. Review the files contained in the Docker directory
- app.py
- DockerFile
- requirements.txt
3. Open a command prompt and cd into the local directory containing your files
- cd C:\Users\{user}\Documents\Piper-2020\Day 2\Docker
4. Type the following command and observe the output
- docker build –t helloworld .
5. Type this command to check that the container image was built successfully
- docker image ls
6. Type this command to start the container and run the Python application
- docker run -p 80:80 helloworld
7. Open a web browser and go to the following URL: http://localhost
