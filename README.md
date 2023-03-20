# Dockerized MENTHU
created by Ryo NIWA

## How to use menthu_docker
```bash=
docker pull geedrn/menthu:latest
docker run --rm -dp 3838:3838 geedrn/menthu:latest
```
After exectution, go to http://localhost:3838

## For people who want to make your own image
```bash=
# download menthu_set.zip and open it
cd menthu_set
docker build . -t IMAGE_NAME
```

## Reference
Docker file was modified from the original repository of MENTHU.
https://github.com/Dobbs-Lab/MENTHU

## MENTHU_set
menthu_set.zip includes the components of rocker/shiny and original MENTHU scripts.
Users can simply download the zip file, defrost it and then docker build in the directory to make a new image.
Some features from rocker/shiny was adjusted to have localhost correctly and debug the error mainly from rentrez package on CRAN.

https://github.com/rocker-org/shiny
