## Jobly Backend

1.  Clone this repository and `cd` into it
2.  `npm install`
3.  `npm run seed` to create db and add in dummy data
4.  `npm start`

In order to access the actual job search pages:
1.  Use dummy account: Username (testuser), Password (password)
2.  Create an account using the signup feature

Troubleshooting Heroku Issues:

When doing [heroku pg:psql < data.sql], you may run into some issues with table conflicts.
If you encounter this issue, it may be because you already have an existing database that is causing
conflicts. To solve this, run [heroku pg:reset DATABASE_URL] in the CLI, then rerun [heroku pg:psql < data.sql]
