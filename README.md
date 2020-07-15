# heaf-demo
HEAF - DigitalOcean Industry Immersion Demo Project

## Deployment
First, create a droplet in [DigitalOcean Cloud](https://cloud.digitalocean.com). Use a password, such as `HEAF2020DO`.

Next, log into the droplet as the root user with:
```
$ ssh root@<ip>
(enter the password and hit <enter> to log in)
```

Install nginx on the machine:
```
# apt update && apt install nginx
```

Lastly, copy the web files to the remote droplet where nginx expects them:
```
$ scp final/* root@<ip>:/var/www/html/.
```

