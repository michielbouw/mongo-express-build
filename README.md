## MongoDB UI setup on dokku

From Mongo express: https://github.com/andzdroid/mongo-express

### Make sure your mongoDB is availible
And check the settings for connecting the mongoDB in the 'config.js' file.

### Push these files to Dokku to create a container

````shell
git remote add mongo-express dokku@<ip_address_of_droplet>:<app_name>
git push mongo-express master
````

### If necessairy link your mongo container to this container

````shell
dokku mongodb:link <app> <database>
````

### Done
Your mongo DB is now availible on <ip_address_of_droplet>:8081
