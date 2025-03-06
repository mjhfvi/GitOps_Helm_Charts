Source: https://docs.linuxserver.io/images/docker-code-server/#docker-compose-recommended-click-here-for-more-info

docker run -d \
 --name=code-server \
 -e PUID=1000 \
 -e PGID=1000 \
 -e TZ=Etc/UTC \
 -e PASSWORD=password `#optional` \
 -e HASHED_PASSWORD= `#optional` \
 -e SUDO_PASSWORD=password `#optional` \
 -e SUDO_PASSWORD_HASH= `#optional` \
 -e PROXY_DOMAIN=code-server.my.domain `#optional` \
 -e DEFAULT_WORKSPACE=/config/workspace `#optional` \
 -p 8443:8443 \
 -v /path/to/code-server/config:/config \
 --restart unless-stopped \
 lscr.io/linuxserver/code-server:latest
