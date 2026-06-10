# Addy.io

## How to use this repo
Follow all steps and you'll be up and running!

### Step 1
Use a public VPS or another server with port 25 open from the outside.  If you can't send email to the server, this will not work.

### Step 2
Install Docker on your server.

### Step 3
Copy the 3 files (.env, addy.env, and docker-compose.yml) to your server.

### Step 4
Edit the files you copied over.  There are ```<domain>``` and ```<command>```

First Run:
```
touch acme.json
chmod 600 acme.json
docker compose up -d
docker compose logs -f
```
