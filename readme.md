# sales-champ-root

SalesChamp > Root
> It includes
> 
> - docker-compose
> 
> - steps to deploy & review codes

## Step 1 - Clone projects

- Download root project
    - `git clone https://github.com/mustafayelmer/sales-champ-root`
- Download address microservice
    - `git clone https://github.com/mustafayelmer/sales-champ`

## Step 2 - Go to root folder

- `cd sales-champ-root` *to change directory*

## Step 3 - deployment

- `docker-compose up --build` *To start deployment*
- `docker-compose down` *To kill running services*

## Docker compose services

- `address`
  > deploys [sales-champ](https://github.com/mustafayelmer/sales-champ)
  >
  > Dependency: `db`
  >
  > Run at [localhost:8090](http://localhost:8090)
  >
  > Swagger at [swagger-ui](http://localhost:8090/docs)
  >
  > ApiDoc at [swagger-json](http://localhost:8090/docs-json)
  >
  > Secrets:
  > - `HTTP_PORT`=`8090` *# web application port*
  > - `MONGO_CONNECTION`=`mongodb://db:27017/sales-champ` *# mongo-db connection string*
- `db`
  > deploys mongo-db server
  >
  > Port: `27017`

---

### Prepared by

- Mustafa Yelmer
- mustafayelmer(at)gmail.com
- `2021-10-25`