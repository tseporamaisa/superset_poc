## Running service locally

### Prerequisites

1. [install Docker](https://docs.docker.com/engine/install/)

2. [install docker-compose](https://docs.docker.com/compose/install/)

### Run using docker compose

1. close this repo

```bash
   git clone https://github.com/tseporamaisa/superset_poc.git
```   
2. change into project directory

```bash
   cd superset_poc
```
3. run service

```bash
   docker-compose up -d
```

> **_Note:_** above comand runs superset on http://127.0.0.1:8088    

4. Login using credentials bellow  
- username: admin
- password: admin

The deployement includes sample data for testing functionality. Enjoy :slightly_smiling_face:    

## Stopping the service    
    
### stop service without clean-up   
```bash
   docker-compose down 
```    
### stop service with clean-up   
```bash
   docker-compose down -v --rmi all --remove-orphans
```
> **_Note:_** above command will remove all volumes, delete images and dangling stuff defined by the compose file