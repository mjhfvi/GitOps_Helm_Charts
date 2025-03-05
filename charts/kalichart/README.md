helm install -f values.yaml kali-linux .

kubectl --namespace NAMESPACE port-forward $POD_NAME 8080:$CONTAINER_PORT

helm uninstall kali-linux
