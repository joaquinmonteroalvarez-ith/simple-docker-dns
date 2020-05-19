# simple-docker-dns

pre-requisite:
remove any service that is listening on port 53

1. create env file
```
mv .env.example .env
```

2. Open the config with vi 
```
vi dnsmasq.conf
```
3. Replace every YOURPRIVATEIP for your private ip. e.g:
```
:%s/YOURPRIVATEIP/192.168.0.23
```
4. Run it
```
docker-compose up -d
```
