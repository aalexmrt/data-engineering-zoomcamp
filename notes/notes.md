# Run postgres docker container

docker run -it \
 -e POSTGRES_USER="root" \
 -e POSTGRES_PASSWORD="root" \
 -e POSTGRES_DB="ny_taxi" \
 -p 5432:5432 \
 -v /Users/alexmartinez/Development/zoom_course/ny_taxi_postgres_data:/var/lib/postgresql/data \
 postgres:13


# Access to psql
 myenv ❯ myenv/bin/pgcli -h <container_name>.orb.local -p 5432 -u root -d ny_taxi