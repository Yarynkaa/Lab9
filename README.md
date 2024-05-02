lab 9 yaryna

## Start the instance.cmd
## Launch command prompt cmd

## Start a Python server:
python3 -m http.server

## Open a separate command prompt window
## Command to connect to a remote server:
ssh -i C:\Users\Yaryna\devOps\lab2.pem -L 5566:127.0.0.1:2375 ubuntu@<ip>

## Open a new command prompt window
## Command to create an image:
docker -H localhost:5566 build -t nginx .

## Command to launch a new container:
docker -H localhost:5566 run -d -p 80:80 nginx

## Display a list of all Docker images:
docker -H localhost:5566 images

## Display a list of all active Docker containers on the Docker server:
docker -H localhost:5566 ps
