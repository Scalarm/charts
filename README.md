# charts
Helm charts for Scalarm

----Summary-----

A chart with scalarm has been created. It includes scalarm dependencies - mongodb and redis.
You can install scalarm on Kubernetes cluster easily with helm tools. 
Scalarm installation is described here: https://github.com/Scalarm/charts/wiki/Setup
The chart uses image scalarm/experiment-manager:1.0.2 which is based on image kliput/scalarm:intern17-1 but additionally it has config files inside.
User's account is created automatically.
You can change values of dependencies in values.yaml. Additionally environment variables and user's account data are available in values.yaml.
Kubernetes cluster has to have dns activated. How to enable dns on your Kubernetes cluster: https://github.com/kubernetes/kubernetes/tree/master/cluster/addons/dns

Future works:
1. make charts of scalarm worker, experiment supervisor and data explorer
2. Add rest of scalarm components - scalarm worker, data explorer and experiment supervisor
3. Scaling 