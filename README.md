## Docker

```bash
docker-compose up -d
```

```bash
docker-compose exec mysql bash
```

```sql
mysql -u root -p products
```

```sql
root
```

```sql
create table products(id varchar(255), name varchar(255), price float);
```

## Kafka

```bash
docker-compose exec kafka bash
```

```bash
kafka-topics --bootstrap-server=localhost:9092 --topic=products --create
```

## Go

```bash
docker-compose exec goapp bash
```

```bash
go run cmd/app/main.go
```

**After Call HTTP Methods**

```bash
docker-compose exec kafka bash
```

```bash
kafka-console-producer --bootstrap-server=localhost:9092 --topic=products
{ "name": "My Product 2", "price": 200 }
```
