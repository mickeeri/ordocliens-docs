# Deploy app

### Postgressql
[Installera PostgreSQL på Ubuntu](http://www.postgresql.org/download/linux/ubuntu/)

* Skapa filen pddg.list: `sudo touch /etc/apt/sources.list.d/pgdg.list`
* Öppna den med `sudo nano /etc/apt/sources.list.d/pgdg.list`
* Lägg till raden `deb http://apt.postgresql.org/pub/repos/apt/ trusty-pgdg main`
* 
```
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | \
  sudo apt-key add -
sudo apt-get update
```
```
sudo apt-get install libpq-dev
```
```
apt-get install postgresql-9.4
```
#### Kom åt postgresql
```
sudo -u postgres psql postgres
```
Ange nytt lösen.
```
postgres=# \password
```
Skapa ny användare
```
create user lawfirm with password 'MY_PASSWORD';
```

Om det inete går att logga in med user
http://stackoverflow.com/questions/18664074/getting-error-peer-authentication-failed-for-user-postgres-when-trying-to-ge

/l för att se alla databaser.
/du för att se alla användare.

#### ssh key
ssh-keygen på lokala
ssh-copy-id demo@SERVER_IP_ADDRESS


Skapa databas
```
create database lawfirm_production owner lawfirm;
```
`Ctrl+D` för att avsluta.

Om man vill skicka mail:
https://youtu.be/pgWWUrI9ZCs?t=5m47s

#### Nodejs
https://nodejs.org/en/download/package-manager/
```
curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
sudo apt-get install -y nodejs
```
#### Skapa ny användare
adduser deployer --ingroup admin
Byt till den användaren
su deployer

#### Installera rbenv
```
curl https://raw.githubusercontent.com/fesplugas/rbenv-installer/master/bin/rbenv-installer | bash
```
Eller enl
https://www.digitalocean.com/community/tutorials/how-to-install-ruby-on-rails-with-rbenv-on-ubuntu-14-04

Installera bundler
gem install bundler --no-ri --no-rdoc
rbenv rehash
bundle -v


https://www.digitalocean.com/community/tutorials/deploying-a-rails-app-on-ubuntu-14-04-with-capistrano-nginx-and-puma

### Github
cat ~/.ssh/id_rsa.pub


cap production deploy:initial

cap production deploy

Starta om server
sudo service nginx restart

### Använbara kommandon
Logga in
`ssh deployer@188.166.165.105`

starta om servern `sudo shutdown -r now`
