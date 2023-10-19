# Database containers

## Oracle

1. Visit https://container-registry.oracle.com/ and create your new account.

2. Select database, after enterprise and Sign in.

3. Accept the License and test if the docker login is working fine or not.

	```
	docker login container-registry.oracle.com
	Username: example@site.io
	Password:
	Login Succeeded
	```

4. Execute docker `docker-compose up -f oracle.yml`

5. Access to container `docker exec -it database-containers_oracle-db_1 sh`

6. Access to database: `sqlplus` o `sqlplus system@localhost1521/ORCLCDB`
