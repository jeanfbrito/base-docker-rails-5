# Base Docker Rails Project

Run the command:
```
docker-compose run web bundle exec rails new . --force --database=postgresql

docker-compose build
```

Modify the file: database.yml

```
host: postgres
username: postgres
password: postgres
```

Run migrations:
```
docker-compose run web bin/rake db:create db:migrate
```

Execute:
```
docker-compose up
```
