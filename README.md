Cybercommons API 
=======

## DEVELOPMENTAL AT THIS POINT!!!


The Cybercommons framework is a Django Rest Framework API. The API leverages MongoDB to provide a Catalog and Data Store for storing metadata and data within a JSON document database. The API also includes Celery which is an asynchronous task queue/job queue based on distributed message passing.

DEVELOPMENTAL AT THIS POINT! This is not an offical release. Please experiment and provide Github Issues or a  Pull Request with added enhancements. 


## Requirements

* Docker
* Docker Compose
    * `pip install docker-compose`
* OpenSSL

## Installation

1. Initialize

        $ git clone <git repo url>
        $ cd cybercommons/dc_config
        $ ./gensslkeys
        $ ./initializeCybercomDB
        $ cd ..

2. Edit values within dc_config/cybercom_config.env
3. Build and Deploy

        $ docker-compose build
        $ docker-compose up -d 

4. API running http://localhost:8080
    * Username: admin
    * Password: admincybercom

5. Kill

        $ docker-compose down

## TODO

1. NGINX config 
1. JWT PAY-LOAD
1. Integration with Kubernetes
