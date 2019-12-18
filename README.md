VIT Linux User Group's Official Website

How to reproduce

1. git clone https://github.com/AbhinavMir/VITLUG-website
2. install npm, sqlite3 and node using choco or sudo or even GUI installation
3. npm install strapi@alpha -g (similarly for yarn if you have)
4. cd <directory of git cloned files>
5. strapi develop


Present Issues:-

https://hidden-earth-32986.herokuapp.com/

Present problems on the website:
1) Not responsive for some reason
2) Database I chose during development was SQLite, but heroku does not support SQLite

Reasons for choosing SQL:-
I was using DB Browser for SQLite which made it easy to import CSV of recruitment results.
SQLite is also very lightweight

Possible solutions:-
1. Migrate from SQLite to Postgres (We can use a converter for .db, but changing infra is something I don't understand rn)
2. Rebuild the entire thing in Mongo /Postgres (not very hard, but I'm not able to go beyond creating new strapi with mongo/PG since it is defaulting to sqlite3, this is a sys error)
