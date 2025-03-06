Source: https://github.com/raonigabriel/web-terminal

docker run --rm -p 7681:7681 raonigabriel/web-terminal:latest

kubectl port-forward $(kubectl get pods --selector "app.kubernetes.io/name=webterminal" --output=name) 7681:7681
