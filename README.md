[![Build Status](https://travis-ci.org/devotis/db-migrate-mssql.svg?branch=master)](https://travis-ci.org/devotis/db-migrate-mssql)
[![Dependency Status](https://david-dm.org/devotis/db-migrate-mssql.svg)](https://david-dm.org/devotis/db-migrate-mssql)
[![devDependency Status](https://david-dm.org/devotis/db-migrate-mssql/dev-status.svg)](https://david-dm.org/devotis/db-migrate-mssql#info=devDependencies)


# db-migrate-mssql
mssql driver for [node-db-migrate](https://github.com/db-migrate/node-db-migrate)

I started this repo from a fork of https://github.com/db-migrate/pg . Took me about half a day to build it, and it's working. [jpinkster] added support for transactions which secures migration state which I merged in today (version 1.1.0).

There is another db-migrate-mssql package (https://github.com/ryd0rz/db-migrate-mssql) that existed before this one. It's published on npm as `db-migrate-mssql`. That is the also the one that node-db-migrate canonically uses when configuring driver: "mssql". I'm not sure of the quality of that package. At first it wasn't working but got fixed recently supposedly.

If you'd like to use this one as an alternative, make sure to do the following. Add this to your package.json and than yarn/npm install:

`"db-migrate-mssql": "https://github.com/devotis/db-migrate-mssql",`

So, don't do yarn add @devotis/db-migrate-mssql for now, and if you already did, remove the line "@devotis/db-migrate-mssql": "...", from your package.json.


## Installation

This is how you would install and use once the feature is added to node-db-migrate that would allow you to appoint another repo as the driver. This request is formulated here: https://github.com/db-migrate/node-db-migrate/issues/593#issuecomment-483039315

```
yarn add @devotis/db-migrate-mssql
```

```
npm install --save @devotis/db-migrate-mssql
```
