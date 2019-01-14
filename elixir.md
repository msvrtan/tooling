# Elixir


Run migrations: `mix ecto.migrate`
Drop database: `mix ecto.drop`
Create database: `mix ecto.create`

Install PostgreSQL cli client (https://websiteforstudents.com/installing-postgresql-10-on-ubuntu-16-04-17-10-18-04/)
```
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ $(lsb_release -sc)-pgdg main" > /etc/apt/sources.list.d/PostgreSQL.list'

apt-get install postgresql-client-10
```

Connect to database
```
psql -h cadera_db -U postgres cadera_dev
```

Show tables
```
\dt
```

Toggle expanded view (show each record as rows of data)
```
\x
```

Describe table in PSQL
```
\d+ conferences;
```

Exit psql
```
\q + ENTER
```


