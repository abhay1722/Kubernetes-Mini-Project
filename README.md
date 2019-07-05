# Kubernetes Mini Project


#### Please refer to https://hub.docker.com/r/abhay1722/node-red for the images used to implement this project and the appropriate build instructions to generate build and test artifacts.

### Follow the steps to setup docker-compose for node-red
  *	Install docker-compose from repository
  *	Use the docker-compose.yaml from the attached package contents.
  *	Run the command `docker-compose up`. You can then access the Node-RED editor by pointing your browser at http://localhost:1880

### Follow the steps to setup Kubernetes and Helm for node-red
  *	Install kubernetes on the system. Make sure all the pods are in `Running` state.
  *	Copy the yaml files provided in the `node-red` directory.
  *	Run `kubectl apply -f deployment.yaml` and `kubectl apply -f service.yaml`
  *	Check if the service is running using `kubectl get svc`.
  *	You can then access the Node-RED editor.
  *	Install Helm and Tiller on the system.
  *	Make sure the `tiller-deploy` pod is in the running state.
  *	Helm create a starter directory structure for the helm chart 
  *	Replace the Kubernetes artifacts written by you in the helm chart.
  *	Run `helm install –name node-red-helm-chart node-red/charts/` to install the helm charts for node-red.
  *	Use the `node-red-chart-0.1.0.tgz` file , obtained using `helm package <chart name>`, with which the charts can be installed.
  *	You can then access the Node-RED editor by running the steps specified on the command line.

_**Note**: This is a sample project used to depict the working of Kubernetes setup._
