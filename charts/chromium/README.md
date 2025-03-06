Source: https://docs.linuxserver.io/images/docker-chromium/#docker-compose-recommended-click-here-for-more-info

docker run -d \
 --name=chromium \
 --security-opt seccomp=unconfined `#optional` \
 -e PUID=1000 \
 -e PGID=1000 \
 -e TZ=Etc/UTC \
 -e CHROME_CLI=https://www.linuxserver.io/ `#optional` \
 -p 3000:3000 \
 -p 3001:3001 \
 -v /path/to/config:/config \
 --shm-size="1gb" \
 --restart unless-stopped \
 lscr.io/linuxserver/chromium:latest
