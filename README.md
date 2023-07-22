Linode Tools
============

Inspired by my need to make a dynamic DNS setup at home, and I didn't want to involve any annoying existing spammy services I've seen (maybe there are good ones?), I made this.

Most of the tools read credentials out of a .env file. Run them without arguments for usage.

Setup
=====
Copy `sample.env` into `.env`, modify the fields as needed.

lido
----
Make Linode API calls. Reads stdin for HTTP verbs that need a body.

status
------
Look up the domain name and record specified in .env to get its current state.

get-domain-record
-----------------
Look up domain name and record specified on cli, outputs the Linode domain ID and domain record ID.

update-up
---------
Get your current public IP. If it has changed since last run, update the record configured in .env with the new IP address.