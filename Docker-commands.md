### Build container image

`docker build -t bytebank:latest .`

### Tag container image

`docker tag bytebank:latest <username>/bytebank:latest`

### Push container image

`docker push <username>/bytebank:latest`

### Run container with specific image and port mapping

`docker run -p 3000:3000 bytebank:latest`