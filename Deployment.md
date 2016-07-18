# Publicera applikation

### Beskrivning
Processen som beskrivs nedan består i en beskrivning av hur jag har gått till väga för att publicera applikationen på en VPS bestående av Ubuntu 14.04.4 x64.

### 1. Logga in på VPS och skapa ny användare 
[Initial Server Setup with Ubuntu 14.04](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-14-04)

[Additional Recommended Steps for New Ubuntu 14.04 Servers](https://www.digitalocean.com/community/tutorials/additional-recommended-steps-for-new-ubuntu-14-04-servers)


### 2. Installera Ruby on Rails
För att installera Ruby och Ruby on Rails används följande instruktioner:

[Setup Ruby On Rails on Ubuntu 14.04 Trusty Tahr](https://gorails.com/setup/ubuntu/14.04)

Jag valde att använda `rvm` och `Ruby 2.3.1`.

För Rails utan dokumentation:
`--no-ri --no-rdoc`

### 3. Installera PostgreSQL databas

För att installaera databasen använde jag instruktionerna på följande sida:

[PostgreSQL Linux Downloads (Ubuntu)](http://www.postgresql.org/download/linux/ubuntu/)

#### Steg för steg
###### 1. Skapa en pgdg.list-fil med.
```
sudo touch /etc/apt/sources.list.d/pgdg.list
```
###### 2. Öppna filen med
```
sudo nano /etc/apt/sources.list.d/pgdg.list
```
###### 3. Lägg till raden
```
deb http://apt.postgresql.org/pub/repos/apt/ trusty-pgdg main
```
###### 4. Kör
```
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | \
  sudo apt-key add -
sudo apt-get update
```
###### 5. Installera dependencies
```
sudo apt-get install libpq-dev
```
###### 6. Installera postgres
```
sudo apt-get install postgresql-9.4
```
###### 7. Logga in
```
sudo -u postgres psql postgres
```
###### 8. Ange nytt lösen. (Frivilligt)
```
postgres=# \password
```
###### 9. Skapa ny användare
```
postgres=# create user lawfirm with password 'MY_PASSWORD';
```
###### 10. Skapa databas. Ibland var jag tvungen att skapa databas först. Ibland skapas den av rails automatiskt.
```
postgres=# CREATE DATABASE lawfirm_development WITH OWNER micke ENCODING 'UTF8' TABLESPACE = pg_default LC_COLLATE 'sv_SE.UTF-8' LC_CTYPE 'sv_SE.UTF-8'  TEMPLATE template0;
```
#### Språkinställingar
```
export LANGUAGE=en_US.UTF-8
export LC_ALL=sv_SE.UTF-8
```
```
sudo locale-gen sv_SE
sudo locale-gen sv_SE.UTF-8
sudo dpkg-reconfigure locales
sudo service postgresql restart
```

#### Troubleshooting
Problem med inloggning. Se [följande svar på Stack Overflow](http://stackoverflow.com/questions/18664074/getting-error-peer-authentication-failed-for-user-postgres-when-trying-to-ge)

#### Användbart
Lista på databaser
```
\l
```
Lista på alla roller
```
\du
```
Avsluta
```
\q
```

[Flytta databas från en server till en annan.](http://stackoverflow.com/questions/1237725/copying-postgresql-database-to-another-server)

#### Uppgradera postgres-version
(Upgrading PostgreSQL from 9.3 to 9.4 on Ubuntu 14.04 LTS)[https://medium.com/@tk512/upgrading-postgresql-from-9-3-to-9-4-on-ubuntu-14-04-lts-2b4ddcd26535#.38w99ii53]

### 4. Installera NodeJS
Node behövs också. Jag använde följande instruktioner för att installera det:

[Installing Node.js via package manager](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)

### 5. Github och ssh-nyckel
Se _Step 5_ på följande sida:

[Setting up SSH Keys](https://www.digitalocean.com/community/tutorials/deploying-a-rails-app-on-ubuntu-14-04-with-capistrano-nginx-and-puma)

### 6. Publicera applikation med Capistrano, Nginx och Puma.
Jag använde instruktioner _Step 1_ och _Step 6_ på följande länk:

[Deploying a Rails app on Ubuntu 14-04 with Capistrano Nginx and Puma](https://www.digitalocean.com/community/tutorials/deploying-a-rails-app-on-ubuntu-14-04-with-capistrano-nginx-and-puma)

Eftersom filerna `database.yml` och `secrets.yml` inte ska versionshanteras behöver man skapa dem i mappen:
```
/apps/lawfirm/shared/config
```

Klista sedan in följande rad i filen `deploy.rb`:
```
set :linked_files, fetch(:linked_files, []).push("config/secrets.yml", "config/database.yml")
```

### 7. Deployment workflow
1. Commita och pusha ändringar på Github.
2. `cap production deploy`

#### Troubleshooting
Ibland behövdes servern startas om, pga minnesbrist eller att databasen var upptagen.

1. `ssh deployer@remote_host`
2. `sudo shutdown -r now`
3. `cap production deploy`

### Användbart
Starta om nginx `sudo service nginx restart`

Stäng av VPS: `sudo shutdown -h now`

#### Ta bort apache-server om förinstallerad
[Permanently removing apache2](http://askubuntu.com/questions/176964/permanently-removing-apache2)

#### Inställningar ny Ubuntu-server
[Recommended steps for new Ubuntu 14-04 servers](https://www.digitalocean.com/community/tutorials/additional-recommended-steps-for-new-ubuntu-14-04-servers)


#### Brandvägg
[How to setup a firewall with ufw](https://www.digitalocean.com/community/tutorials/how-to-setup-a-firewall-with-ufw-on-an-ubuntu-and-debian-cloud-server)


#### Använd Gmail för t.ex. återställningsmail
[How to set up gmail with your domain](https://www.digitalocean.com/community/tutorials/how-to-set-up-gmail-with-your-domain-on-digitalocean)

#### Barman för backup-server
[How To Back Up, Restore, and Migrate PostgreSQL Databases with Barman](https://www.digitalocean.com/community/tutorials/how-to-back-up-restore-and-migrate-postgresql-databases-with-barman-on-centos-7)

1. Tillåt backup-servern i brandväggen. 
2. Ändra raden till `listen_adress='*'` eller `listen_adress='backup_server_ip'`
3. För att få mappen där databasen finns. Se [länk](http://askubuntu.com/questions/197626/where-is-a-postgresql-9-1-database-stored-in-ubuntu-12-04)
```

```
