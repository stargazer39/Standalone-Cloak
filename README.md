# Cloak-Squid-Docker

Deploy a quick squid proxy with cloak transport..
Primarily made to work with Heroku

```bash
docker run -d --network="host" -v /home/stargazer/configs/cloak/:/config -p 443:443 <image_name>
```
You can edit the config later in configs folder and restart the container

To set parameters manually make a .env file with

```bash
CK_ADMINUID=<uid>
CK_BYPASSUID=<uid>
CK_PRIVATEKEY=<private_key>
PORT=<internal_listening_port>
```
