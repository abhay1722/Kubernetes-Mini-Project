•	Please refer to https://hub.docker.com/r/abhay1722/node-red for the images we used to implement this project and the appropriate build instructions to generate build and test artifacts.
•	Follow the steps to setup docker-compose for node-red
o	Install docker-compose from repository
o	Use the docker-compose.yaml from the attached package contents.
o	Run the command “docker-compose up”. You can then access the Node-RED editor by pointing your browser at http://localhost:1880
•	Follow the steps to setup Kubernetes and Helm for node-red
o	Install kubernetes on the system. Make sure all the pods are in “Running” state.
o	Copy the yaml files provided in the “node-red” directory.
o	Run “kubectl apply -f deployment.yaml” and “kubectl apply -f service.yaml”
o	Check if the service is running using “kubectl get svc”.
o	You can then access the Node-RED editor.
o	Install Helm and Tiller on the system.
o	Make sure the “tiller-deploy” pod is in the running state.
o	Helm create a starter directory structure for the helm chart 
o	Replace the Kubernetes artifacts written by you in the helm chart.
o	Run “helm install –name node-red-helm-chart node-red/charts/” to install the helm charts for node-red.
o	Please find attached a .tgz file of the chart , obtained using ‘helm package <chart name>’, with which the chart can be installed 
o	You can then access the Node-RED editor by running the steps specified on the command line.

