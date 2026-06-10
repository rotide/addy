# Addy.io

### How to use this repo
Follow all steps and you'll be up and running!

### Step 1
You will need to get the following:
- A public facing server with port 25 open and accessible!
  - Most ISPs and quite a few VPS providers block this by default.
- A domain name where you control the DNS records.

### Step 2
Install Docker on your server.

### Step 3
Copy the 3 files (.env, addy.env, and docker-compose.yml) to your server.

### Step 4
Edit the files you copied over.  There are ```<domain>``` and ```<command>``` variables in the files which need to be changed.

### Step 5
Create the acme.json file for SSL certificate storage.
```
touch acme.json
chmod 600 acme.json
docker compose up -d
docker compose logs -f
```

### Step 6
Bring up the container and watch the logs for errors/issues.
```
docker compose up -d
docker compose logs -f
```
