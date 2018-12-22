# micro-node

Node.js structure for microservice

## .env

```
DB_USER=root
DB_PASS=password
DB_DATABASE=database
DB_HOST=3306
DB_DIALECT=mysql

API_LIMIT=50
API_PORT=3000
API_VERSION=v1
```

## Sequelize

Create model

```bash
node_modules/.bin/sequelize model:generate --name User --attributes firstName:string,lastName:string,email:string
```

Create migration

```bash
node_modules/.bin/sequelize db:migrate
```

Create seeder

```bash
node_modules/.bin/sequelize seed:generate --name demo-user
```

Running seeder

```bash
node_modules/.bin/sequelize db:seed:all
```
