# quickstart 
Make sure you have already installed both Docker Engine and Docker Compose and you have a domain name point to your machine. navigate to the root of project and execute

### Testing mode
```
export DOMAIN_NAME=<YOUR_DOMAIN_NAME> && export STAGING=true && docker-compose up 
```
### Production mode
```
export DOMAIN_NAME=<YOUR_DOMAIN_NAME> && export STAGING=false && docker-compose up -d
```
### note
Domain name is used by nginx to generate ssl certificate.
you have only 5 certificat request per week when you use production mode.
