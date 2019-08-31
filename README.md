# Jupyter build

Jupyter build with a bunch of stuff.

## Build

### Pre

```
wget https://download.oracle.com/otn_software/linux/instantclient/193000/instantclient-basiclite-linux.x64-19.3.0.0.0dbru.zip
wget https://download.oracle.com/otn_software/linux/instantclient/193000/instantclient-sqlplus-linux.x64-19.3.0.0.0dbru.zip
wget https://download.oracle.com/otn_software/linux/instantclient/193000/instantclient-sdk-linux.x64-19.3.0.0.0dbru.zip
unzip *.zip
```

`jupyter-repo2docker -E .`

## Pull

```bash
docker run -p 8080:8888 -v ~/Projects/jupyter-bundle/workspace:/home/gavin/workspace gaving/jupyter-bundle:latest
```
