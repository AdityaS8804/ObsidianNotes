"POSTGRES_PASSWORD=mysecretpassword",
			"POSTGRES_USER=postgres",
			"POSTGRES_DB=userdb",
			"PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/17/bin",
			"GOSU_VERSION=1.17",
			"LANG=en_US.utf8",
			"PG_MAJOR=17",
			"PG_VERSION=17.4-1.pgdg120+2",
			"PGDATA=/var/lib/postgresql/data"

docker exec -it postgres-user-crud psql -U postgres -d userdb -c "SELECT * FROM master;"   





docker exec -it <container_name> psql -U <username> -d <database_name> -c "SELECT * FROM master;"


docker exec -it postgres-user-crud psql -U postgres -d userdb -c "\dt master.*"   



docker exec -i postgres-user-crud psql -U postgres -d userdb  < /Users/adityas/Developer/nument-ai/auth-service/src/repository/db/user_schema.sql