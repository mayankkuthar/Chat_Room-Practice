# Chat_Room-Practice

This a practice project for creating a Chatting application. I have created a similar application earlier too, But as we know Heroku free-tier is not available any more from 28th NOV 2023. So, we are switching to different paltform.

## Database Limitations:

### PostgresSQL [Render]

- Free instances do not support backups.
- A free database expires 90 days after creation.
- Only one free PostgreSQL instance can be active for any given Render user

### Solution to overcome obove mentioned points of Database:

- So, We will create a Backup script in python which will download all the data and save all the data on local system on regular intervals. Now we know Database expires after 90 days. So we will select 49 days as a time-period for regular backups.

```
Maths Behind it:
Primes of 90 are 2,5 and 3 so we select 7  (minimum prime non-factor value)
Now, For n=2 [7ⁿ] as 49 is the largest less than 90 for 7's power.
```