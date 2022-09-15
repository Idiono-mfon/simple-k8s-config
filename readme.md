## Create a secret component

Create secret first
Apply the scret (kubectl apply -f mongo-secret.yaml)

## MongoDB depolyment for pod/replicaset

Create the mongoDB.yaml deployment
Reference the secret on our configuration file
Then apply it (kubectl apply -f mongo.yaml)

## Config Map

Create config map componet using the mongoconfigmap.yaml

Then apply it (kubectl apply -f mongo-configmap.yaml)

## Mongo Express Web Interface

Create the Mongo Express POD/replicaset and apply it

Then apply it (kubectl apply -f mongo-express.yaml)

## Assign a public IP address to external service

Use the command below to get the IP addess of minikube and acess it wih the port assigned

minikube ip

or

kubectl get node -o wide
