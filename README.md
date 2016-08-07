# template-spring-boot-data-jpa-postgresql-docker
A template Spring Boot JPA project with postgresql as database and easy start up with Docker Compose

## postgresql 

    $ docker run --name tmpl-postgres -e POSTGRES_PASSWORD=mysecretpassword -e POSTGRES_DB=tmpl -v /etc/localtime:/etc/localtime:ro -p 25432:5432 -d postgres:9.5.3
    $ docker run -it --rm --link tmpl-postgres:postgres postgres psql -h postgres -U postgres 
    postgres # select current_timestamp;  
