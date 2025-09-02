### Build container image

`docker build -t bytebank:latest .`
`docker build -t bytebank-investments:latest .`

### Tag container image

`docker tag bytebank:latest <username>/bytebank:latest`
`docker tag bytebank-investments:latest <username>/bytebank-investments:latest`

### Docker Hub login

`docker login`

### Push container image

`docker push <username>/bytebank:latest`
`docker push <username>/bytebank-investments:latest`

### Run container with specific image and port mapping

`docker run -p 3000:3000 bytebank:latest`
`docker run -p 3001:3000 bytebank-investments:latest`