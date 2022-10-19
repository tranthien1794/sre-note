```
docker run -d \
    --name=chromium \
    -p 5800:5800 \
    -v /docker/appdata/chromium/Downloads:/config/Downloads:rw \
    --shm-size 2g \
    overclockedllama/docker-chromium
done
```