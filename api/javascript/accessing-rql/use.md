---
layout: api-command 
language: JavaScript
permalink: api/javascript/use/
command: use 
github_doc: https://github.com/rethinkdb/docs/edit/master/2-query-language/api/javascript/accessing-rql/use.md
io:
    -   - connection
        - undefined
related_commands:
    connect: connect/
    reconnect: reconnect/
    close: close/
---

# Command syntax #

{% apibody %}
conn.use(dbName)
{% endapibody %}

# Description #

Change the default database on this connection.

__Example:__ Change the default database so that we don't need to specify the database
when referencing a table.

```js
conn.use('heroes')
```