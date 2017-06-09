# rpwm-dockerized

Dockerized rhodecode packagist webhook middleware

# rpwm

Check https://github.com/darneta/rpwm

### ENV variables

`PACKAGIST_USER` - packagist username  
`PACKAGIST_TOKEN` - packagist API Token  
`WEBHOOK_TOKEN` - Rhodecode webhook "Secret Token"  
`PACKAGIST_URL` - default "https://packagist.org"  
`APP_PORT` - default 80  

### Run

```bash 
docker run \
-e PACKAGIST_USER=someuser \
-e PACKAGIST_TOKEN=secrettoken \
-e WEBHOOK_TOKEN=rhodecodesecretoken \
--name rpwm \
darneta/rpwm
