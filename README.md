# kubeplugin
test bash script as plugin to kubectl

test output example:
Resource: nodes in Namespace: kube-system with Name: argocd-control-plane usage of CPU is: 234m and Memory: 2%

requrements:
kubernetes cluster
metric server 
kubectl

instruction of usage:
1. Place script to some folder where $PATH can read it.
2. If name of script starts from kubectl- (kubectl-script) - second part will be readed like command for kubectl.
For example:
kubectl script

required arguments for plugin:
For correct work of plugin You need to add in command two arguments;
1) resource type
2) namespace name

For example:
kubectl script pods staging
