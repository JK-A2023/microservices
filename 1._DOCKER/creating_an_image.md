# How to create an Image in Docker:

1. Create a directory:

```
mkdir my_docker_folder && cd my_docker_folder
```

2. Create the Dockerfile:

```
nano Dockerfile
```

3. Add Docker content, depending on file.

E.g.:

```
FROM node:latest

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY . .

# Install application dependencies
RUN npm install

# Copy the rest of the application code to the contain

# Expose the port your Node.js app listens on (e.g., 3000)
EXPOSE 3000

# Define the command to start your Node.js application
CMD ["node", "app.js"]
```

4. Test image:

```
docker build -t sparta_app
```

5. Tag docker with username so it knows where to be pushed to:

```
docker tag sparta_app jka2023/sparta_app
```

6. Push to docker:

```
docker push jka2023/sparta_app
```