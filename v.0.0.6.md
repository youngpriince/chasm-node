# Update Scout to v0.0.6

```sh
docker stop scout
```
```sh
docker rm scout
```
```sh
# pull the latest image
docker pull chasmtech/chasm-scout:latest
```
Note: make sure your `.env` file is up-to-date
## Run updated scout
```sh
docker run -d --restart=always --env-file ./.env -p 3001:3001 --name scout chasmtech/chasm-scout
```
## Check logs
```sh
docker logs scout
```
