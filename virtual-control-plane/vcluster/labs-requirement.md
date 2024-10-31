# Labs Requirements 
* a local kubernetes distribution (minikube, rancher, docker-desktop) 
* a network plugin enabled
* the ingress plugin enabled
* kubectl installed
* helm installed

## If you are using minikube, just run

```
minikube start --cni calico --addons ingress --extra-config=apiserver.enable-admission-plugins=PodNodeSelector,LimitRanger,ResourceQuota,MutatingAdmissionWebhook,ValidatingAdmissionWebhook
```
