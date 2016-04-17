# 1dv42e-me222wm-dokumentation
### Körinstruktioner

Skapa database.yml
Skapa secret.yml

`$ sudo -u postgres psql postgres`
`postgres=# \password postgres`

`Enter new password:`
`Enter it again:`

`su - postgres`
`psql`
`create role myapp with createdb login password 'password1';`
(glöm inte semikolon)
`Ctrl+D` för att avsluta.


Port: 5432

#### How to install phantomJS
https://gist.github.com/julionc/7476620
