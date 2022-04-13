## Running service locally

### Prerequisites

1. [install Docker](https://docs.docker.com/engine/install/)

2. [install docker-compose](https://docs.docker.com/compose/install/)

> **_Note:_** if using Mac, docker desktop for Mac includes docker-compose out of the box so no need to install separately.

### Run through setup script

1. clone this repo

```bash
   git clone https://github.com/tseporamaisa/superset_poc.git
```   
2. change into project directory

```bash
   cd superset_poc
```
3. run superset service

```bash
   bash setup.sh start
```

> **_Note:_** above comand runs superset on http://127.0.0.1:8088    

4. Login using credentials bellow  
- username: admin
- password: admin

The deployement includes sample data for testing functionality. Enjoy :slightly_smiling_face:    

## Stopping the service    
    
### stop service without clean-up   
```bash
   bash setup.sh stop 
```    
### stop service and clean-up   
```bash
   bash setup.sh cleanup
```
> **_Note:_** above command will remove all volumes, delete images and dangling stuff defined by the compose file