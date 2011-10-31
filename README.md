This is a simple template to allow you to db:push from a sqlite or mysql db to a heorku postgresql db. It's only needed if your app isn't a ruby app.

Use:
modify config/database.yml to contain the proper database credentials

$ bundle install

$ bundle exec heroku db:push --app app-name

If you need a shared database on heroku:

$ heroku addons:add shared_database --app app-name

warning: running taps in this fassion will overwrite the database at DATABASE_URL on heroku.

