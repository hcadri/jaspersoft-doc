# Jaspersoft Server in Docker containers
## Setup
copy TIB_js-jrs_8.1.0_bin.zip to /sources
```sh
cd script && ./unpackWARInstaller.sh
cd ..
docker-compose build
docker-compose run jasperserver-buildomatic
docker-compose up -d jasperserver-webapp
```
## Troubleshouting
exec /usr/local/scripts/entrypoint.sh: no such file or directory
*.sh files should have `LF` line endings