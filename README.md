# Change a Password for PostgreSQL on Linux via Command Line
## Switch to the PostgresSQL User: postgres
If you’re working from a default PostgreSQL installation, then PostgreSQL will be configured with the user postgres.

Since we’re logged in as root, and we’re assuming that root doesn’t have a user for PostgreSQL, switch to the default PostgreSQL user: postgres:

```commandline
su - postgres

psql
```

## Add/Change the Password for the PostgreSQL User: postgres

```commandline
\password
```

Enter your new password, and then enter it again to confirm it:

```commandline
Enter new password:
Enter it again:
```

```commandline
\q
```

Quick Run

You can do all the step one in exactly one command:

```commandline
su -c "psql" - postgres
```