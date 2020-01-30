1. Check that the Kubernetes cluster is running and available
- kubectl get deployment
2. Type the following command and observe the output
- kubectl create deployment helloworld --image=theocrithary/helloworld
  - Note: we are using the same image we built in Lab 01, except this version has been pushedto a repository on Docker Hub. i.e. https://hub.docker.com/repository/docker/theocrithary/helloworld
3. Type this command to check that the container was deployed to the Kubernetes cluster
- kubectl get deployment
4. Type this command to check that a pod was built and is running succesfully
- kubectl get pods
5. Type this command to expose port 80 and allow external access into the Kubernetes cluster
- kubectl expose deployment helloworld --type=LoadBalancer --port=80
6. Open a web browser and go to the following URL: http://localhost
