---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
## What it does
An app for people who want to know what happens in congress about issues they care about. This program will let you subscribe to E-mail notifications for new bills as they are introduced and current bills as their statuses change. The search uses keyword association to match results against the [ProPublica Congress][proPublica] collection.

## How it works
In order to provide the most timely notifications to users about new bills that might interest them, our application periodically polls the API for new bills and adds them to our database.

It uses a natural language processing API (the Twinword Topic Tagging API) to generate keywords based on the new bills' full text (if available) or title (always available). These keywords are stored in the database entry for each bill. The keywords are used to power the application's notification capabilities as well as its dashboard view, where the application shows recent bills related to a user's monitored topics of interest.

[proPublica]: "https://projects.propublica.org/api-docs/congress-api/"
