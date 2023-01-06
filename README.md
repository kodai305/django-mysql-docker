# django-mysql-docker
for dev environment


## 手順

### コンテナの起動

```
docker-compose build
docker-compose up -d
```

### マイグレーション(どこで実行するべきかは要検討)

```
docker-compose exec web bash
python3 manage.py makemigrations app
python3 manage.py migrate
```