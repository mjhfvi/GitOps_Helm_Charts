Source: https://docs.linuxserver.io/images/docker-kali-linux/#docker-compose-recommended-click-here-for-more-info

helm install -f values.yaml kali-linux .

kubectl --namespace NAMESPACE port-forward $POD_NAME 8080:$CONTAINER_PORT

helm uninstall kali-linux

docker run -d \
 --name=kali-linux \
 --security-opt seccomp=unconfined `#optional` \
 -e PUID=1000 \
 -e PGID=1000 \
 -e TZ=Etc/UTC \
 -e SUBFOLDER=/ `#optional` \
 -e TITLE="Kali Linux" `#optional` \
 -p 3000:3000 \
 -p 3001:3001 \
 -v /path/to/data:/config \
 -v /var/run/docker.sock:/var/run/docker.sock `#optional` \
 --device /dev/dri:/dev/dri `#optional` \
 --shm-size="1gb" `#optional` \
 --restart unless-stopped \
 lscr.io/linuxserver/kali-linux:latest
