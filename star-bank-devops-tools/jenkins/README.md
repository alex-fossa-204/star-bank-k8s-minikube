STEP_1: Create a Namespace config file for DevOps tools nad services if not exists.
[`kubectl create namespace star-bank-devops-tools`]

STEP_2: Create a Jenkins Account config file, set up role and username
[`kubectl apply -f service-account-config.yaml`]

STEP_3: Create a Jenkins Persistent Volume config file if you want to store jenkins data locally
[`kubectl create -f persistent-volume-config.yaml`]

Step 4: Create a Deployment config file to deploy jenkins instance in a current node
[`kubectl apply -f deployment-config.yaml`]

Step 5: Create a Service Network config file to deploy jenkins instance in a current node
[`kubectl apply -f service-network-config.yaml`]

FULL_INSTRUCTION: [`link`](https://www.jenkins.io/doc/book/installing/kubernetes/)