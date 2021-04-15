## Dockerizing MERN Stack Application 

### Prerequisites:

You must have Docker Installed in your System !

### How to run the App :

##### In Development Mode :

Run the app using :

`$ docker-compose up --build --remove-orphans`

or

`$ docker-compose up -d`

Above command will start the services on (-d) detach mode (similar like running the app in background)

Then you can check the status of the containers by running:

`$ docker ps`

The App should be App :

visit client : http://localhost:3000

visit server : http://localhost:8080

To check the status of the running containers :

`docker-compose ps`

### Build the image for server :
`docker build -t myapp-server:1 .`
`docker images`
`docker run --name "myapp-server" -p 80:8080 myapp-server:1`
`docker ps`

### Build the image for client :
Build Client Image:
`docker build -t myapp-react:v1 .`
Run the container
`docker run -p 3000:3000 myapp-react:v1 `