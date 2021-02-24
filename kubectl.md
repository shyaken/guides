# Windows

### gcloud sdk
Download & install gcloud sdk: https://cloud.google.com/sdk/docs/install


### kubectl
Download kubectl exe: https://kubernetes.io/docs/tasks/tools/install-kubectl/


### config:
gcloud auth login
gcloud config set project <project-name>
gcloud container clusters get-credentials <project-name> --zone=<project-zone>

#### Rename your local context (Optional)
kubectl config rename-context $(kubectl config current-context) <develop-context-name>

#### Then change context to new context
kubectl config set-context <develop-context-name> --namespace=<your-namespace>
