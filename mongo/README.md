# Set up mongodb as StatefulSet
We will deploy the following components for our MongoDB cluster:
* Daemon Set to configure HostVM
* Service Account and ClusterRole Binding for Mongo Pods
* Storage Class to provision persistent SSDs for the Pods
* Headless Service to access to Mongo Containers
* Mongo Pods Stateful Set
* GCP Internal LB to access MongoDB from outside the kuberntes cluster (Optional)
* Access to pods using Ingress (Optional)