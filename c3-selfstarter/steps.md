
# Rails Starter 3 - Self devleop your first real project

heroku create
http://whispering-depths-2018.herokuapp.com/ | git@heroku.com:whispering-depths-2018.git

heroku pg:info
=== HEROKU_POSTGRESQL_BROWN_URL (DATABASE_URL)
Plan:        Dev
Status:      available
Connections: 0
PG Version:  9.1.6
Created:     2012-11-03 14:32 UTC
Data Size:   5.9 MB
Tables:      0
Rows:        0/10000 (In compliance)
Fork/Follow: Unavailable

if you have not pg database, run below cmd to create new pg database:
heroku addons:add heroku-in

postgresql your database:
```
production:
  adapter: postgresql
  database: $DATABASE_URL
  pool: 5
  timeout: 5000
```

db migrate:
heroku run rake db:migrate



