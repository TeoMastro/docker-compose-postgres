# To run the database:
- docker-compose up -d
- go to http://localhost:5050/
- enter PGADMIN_DEFAULT_EMAIL and PGADMIN_DEFAULT_PASSWORD

# To register a new server inside the db
- docker container ls (to get the CONTAINER ID of the postgres image)
- docker inspect CONTAINER ID (to find the IP of the container)
- Then inside the pgAdmin -> Add new Server
- On General tab put a name (e.g. 'test_db')
- On Connection tab enter the IP of the container on Hostname
- Username and passoword: POSTGRES_USER and POSTGRES_PASSWORD

# Reference videos
- https://www.youtube.com/watch?v=qECVC6t_2mU
- https://www.youtube.com/watch?v=eKEzq59FhEw