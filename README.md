## MongoDB UI setup

From Mongo express: https://github.com/andzdroid/mongo-express

### Make sure your mongoDB is availible
And check the settings for connecting the mongoDB in the 'config.js' file.

### Push these files to Dokku to create a container

````shell
git remote add dokku dokku@<ip_address_of_droplet>:<app_name>
git push dokku master
````

### Run

````shell
node app
````

### Done
Your mongo DB is now availible on localhost:8081.



