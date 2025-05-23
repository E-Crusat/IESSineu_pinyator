Aquest repositori s'ha important d'una copia del Pinyator dels Castellers d'Estocolm amb una finalitat educativa a un Institut de Mallorca per ensenyar com fer servir eines de control de versions. Aquest codi NO és correcte, ha rebut canvis en el procés d'ensenyament del control de serveis. Dit d'una altra manera,

# No feu servir aquest codi per montar la vostra pròpia versió del Pinyator

---

# Pinyator

## Source

This application has been developed by [Marrecs de Salt](https://marrecs.cat) and can be found publicly [here](https://gitlab.com/elputorei/Pinyator/). The following repository is a fork of the original and contains minor fixes to be able to run this application with newer versions of PHP and MySQL.

## Local setup

### Requirements

- Docker
- Docker compose

### Setup

1. Create the containers.

```shell
docker-compose up -d
```

2. If it's the first time, migrate the database.

```shell
mysql -u pinyator -ppinyator -h 0.0.0.0 pinyator < pinyator/src/Pinyator_BD.sql
```

3. You can now reach the application in the following URL.

[http://localhost:8100/pinyator/Pinyator.php](http://localhost:8100/pinyator/Pinyator.php)

4. After development, turn down the containers.

```shell
docker-compose down
```
