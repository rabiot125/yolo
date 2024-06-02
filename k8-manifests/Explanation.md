#Project overview

## Technologies Used

- **Docker**: Containerization of frontend, backend, and database.
- **Kubernetes**: Orchestration and management of Docker containers.
- **React**: Frontend client framework.
- **Node.js**: Backend server runtime.
- **MongoDB**: NoSQL database for data storage.
- **kubectl**: Command-line tool for Kubernetes.

## Deployment Steps

### Prerequisites


- Kubernetes cluster configured (e.g., minikube, GKE).

### Steps

1. **To setup run deployment in cluster **
   ```sh
	kubectl apply -f backend-deployment.yaml
	kubectl apply -f backend-service.yaml
	kubectl apply -f client-deployment.yaml
	kubectl apply -f client-service.yaml
	kubectl apply -f mongodb-service.yaml
	kubectl apply -f new-storage-class.yaml
	kubectl apply -f mongopv.yaml
	kubectl apply -f mongopvc.yaml
	kubectl apply -f mongodb-statefulset.yaml
2. **Access the Application**

     [frontend](http://34.41.218.34:3000/)

