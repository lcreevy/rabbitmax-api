# RabbitMax API

Free and open source software and hardware IoT platform with HTML5 UI, Node.js HTTP API and MQTT.

## Overview

HTTP API and a simple web interface for DIY (Do It Yourself) IoT (Internet of Things) which use MQTT to communicate between each other. Short video demonstraion and introduction: https://www.youtube.com/watch?v=HA0AjwYzK5Q

## Getting Started

* Install the web application:

Follow the steps below to install RabbitMax on Ubuntu or Debian:

```bash
$ git clone git@github.com:RabbitMax/rabbitmax-api.git
$ cd rabbitmax-api
$ git clone git@github.com:RabbitMax/rabbitmax-ui.git ui
$ npm install
$ sudo apt-get install mysql-server
$ mysql -u root -p < sql/db.sql
$ mysql -u root -p < sql/data.sql
$ cp api/config-example.json api/config.json
```

* Start the server:

```bash
$ systemctl start mysql
$ nodejs api/index.js
```

* Open a web browser and navigate to [http://localhost:3000/](http://127.0.0.1:3000/).  Log in using username `demo` and password `demo`.
