# Docker commands reference

This repository is a simple point of knowledge for docker commands

## Getting an image

- `docker run` - Basic command to start an image
  - `-d` (deattach) - Able you to start an image and leave the terminal opened
  - `-name` - Set a name for an image, if you don't specify, docker will create one for you
  - `-P` - Set a local port to listen your image
  - `-p` - Specify a local port to your image
  - `-it` - Executing image from terminal

### Example

- `docker run -d -p 12345:80 dockersamples/static-site`
Run image *static-site* signed by *dockersamples* from image port 80 to local port 12345

## Image management

- `docker ps` - Basic command to list active images
  - `-a` - Getting all imagens activated or not
  - `-q` - Getting image IDs
  - `-s` - Getting image sizes

## Start an installed image

- `docker start <id>` - Start an imagem from the ID
  - `-a` - Attach the STDOUT/STDERR and other outputs
  - `-i` - Interactive mode

## Stop an image

- `docker stop <id>` - Stop an imagem from the ID
  - `-t <time-seconds>` - Seconds to wait for stop
