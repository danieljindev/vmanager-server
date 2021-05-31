<p align="center">
  <b>VManager Personal Affairs Management System</b>
  <p align="center">
    <a href="https://github.com/danieljindev/vmanager-client">WEB</a>
  </p>
</p>

## Built with
- [Node.js >= 14](https://nodejs.org/en/)
- [Egg.js](https://eggjs.org/zh-cn/intro/)
- [MySQL](https://www.mysql.com/)
- [Sequelize](https://github.com/sequelize/sequelize)
- [js-ant](https://github.com/xjh22222228/js-ant)

## MySQL Setup
Simple MySQL install and config

```
# Install mysql
sudo apt install mysql-server
systemctl status mysql.service

# Adjusting User Authentication 
sudo mysql
mysql > SELECT user,authentication_string,plugin,host FROM mysql.user;
mysql > ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '123456';

# Create a database for tomato work
mysql > CREATE DATABASE tomato_work

# Later you can login to mysql via
mysql -u root -p
```

## Build Setup
Please configure database information before starting the project in  config/config.default.js

``` bash
# Download
git clone --depth=1 https://github.com/danieljindev/vmanager-server.git

# Install
yarn

# Port: 7003
yarn dev

# Build start
yarn start
```

---

## License
[MIT](https://opensource.org/licenses/MIT)
