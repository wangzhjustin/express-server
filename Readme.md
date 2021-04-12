Express-Server for MHS
===

## Outline

This is the server built for MHS-APP. Because the APIs were written in RESTful style, the IT department in Ming Hui Sheng Enterprise Co., LTD. can easyly jump on this and develop other features.

## Installation

> Built with FreeBSD 12.1, Node.js v14.4.0

1. Install Nodejs.
2. Install pm2 `$npm install pm2`.
3. Clone repository.
4. cd to express-server.
5. Run `$npm install`.
6. create a file userConfig.js in root folder
```
//in userConfig.js

const mysqlConfig = {
    host: 'your host',
    user: 'your user',
    password: 'your password',
    database: 'your database'
}

module.exports = {mysqlConfig};
```

## Usage

`$pm2 start bin/www --watch --max-memory-restart 20M.`

## Appendix and FAQ

:::info
**Find this document incomplete?** Leave a comment!
:::

###### tags: `expressjs`
