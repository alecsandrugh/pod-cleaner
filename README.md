# Pod-cleaner

## Pod specs local image imagePullPolicy: Never
spec:
  template:
    metadata:
      name: hello-world-pod
    spec:
      containers:
      - name: hello-world
        image: forketyfork/hello-world
        imagePullPolicy: Never


## Use docker local repo
minikube docker-env
eval $(minikube -p minikube docker-env)
docker build -t kube .
docker image list

