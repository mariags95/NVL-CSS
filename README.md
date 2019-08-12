**Start Up the APP**

Start MongoDB by running 'mongod' and redis by running 'brew services start redis' (on Mac)

Export mongodb environmental variables:
- 'mongodb_username' for the username of mongodb (if necessary)
- 'mongodb_password' for the pass of mongodb (if necessary)
- 'betbroker_jwtPrivateKey' for jwt private key (12345 for local dev)
- 'auth4admin' for admin middleware authorization (croquetas-para-todos for local dev)
-  DEBUG=app:* for the debug package

- Run run nodemon to continuos relaunch the app of updates.

**TESTING!**

- Running index.js with NODE_ENV=test: NODE_ENV=test node index.js



**When dealing with bets I will need to use fawn (npm i already run)**

Fawn is a libary used for transactions:

 (From the docs):
    _Fawn provides the ability to carry out edits on a mongoDB database as a series of steps. If an error occurs on any of the steps, the database is returned to its initial state (its state before the transaction started). It's based on the two phase commit system described in the MongoDB docs._
 
 (see more on //https://www.npmjs.com/package/fawn)
