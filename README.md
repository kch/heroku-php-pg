# PostgreSQL + PHP on Heroku

This otherwise entirely useless app demonstrates how to connect to your 
Heroku PostgreSQL database in a PHP app.

Long story short, read your connection data from `DATABASE_URL`.

Every time you hard-code the connection info, god kills an octokitten.


# Running this app on Heroku:

Clone it, then create your Heroku app with:

    $ heroku create --stack=cedar

Push your clone to Heroku:

    $ git push heroku master

PHP apps don't get a database by default, so you have to add it manually:

    $ heroku addons:add shared-database

Once that's done, you can visit your app with:

    $ heroku open
