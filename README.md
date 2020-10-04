 # **KubeDev Week**
 
 This project was developed during KubDev week by Fabrício Veronez. 
 
 There are four files because eacho one represent the context given during this week. 
 
 The main applycation is at KubeDev-4 folder.
 
 The main idea is to create docker images, run them in containers and as well use kubernetes to manage the conatiner(S) created. 
 
 We used a node.js application that can be found at https://github.com/KubeDev/api-produto
 
 From that, it was included a Dockerfile, .dockerignore, and kubernetes files for the database and the application (deployment.yaml and service.yaml for each)
 
 To run the container use the following command:
 
 
 *docker container run -d -p 8080:8080 naraguimma/api-produto:v1*
 
 
 To access this container, first you must get your local external IP address (open prompt or type "cmd"in the search box in your start menu to open it, type "ipconfig" and look for "ETHERNET ADAPTER ETHERNET" where you may find all information about your network adapter. Get the number associated with "IPv4 Address ...........: XX.X.XXX.XX")
 
 Go to your browser and type: 
 
 
 
 **XX.X.XXX.XX:8080/api-docs**
 
 
 If you want to remove this container from your list, just type: 
 
 *docker container ls*  ------ get the container ID you want to remove.
 
 
 *docker container rm -f  [paste the container ID here]*
 
 
