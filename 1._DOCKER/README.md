# How to set up and start an application in Docker:

1. Check if it is installed and running:

```
Docker
```

OR 

```
Docker --version
```

## To run NGINX:

```
$ docker run -d -p 80:80 nginx
```

This will download the latest NGINX release and run the application on port 80, forwarding to port 80.
You can access this webpage on your local host, or if running on an EC2, public IP address.

## Checking containers:

```
docker ps
```

This command will list containers, their ID's, and image being used.

## Starting / Stopping containers:

```
docker start <CONTAINER_ID>
```

```
docker stop <CONTAINER_ID>
```

## Removing a container:

```
docker rm <CONTAINER_ID>
```

## Removing an image:

```
docker rmi <IMAGE_ID>
```

## Using Shell with Docker:

```
docker exec -it <CONTAINER_ID> sh
```

If running into error:

```
alias docker="winpty docker"
```

Run the following once in:

```
apt update
```

```
apt upgrade -y
```

```
apt install sudo
```

```
apt install nano
```

