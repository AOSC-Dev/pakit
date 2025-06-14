leaves.sql
===

SQL inquiry to generate a repository-wide list of packages with no reverse
dependencies based on [p-vector](https://github.com/AOSC-Dev/p-vector-rs)'s
database.

Usage
---

After logging onto the repository server, run the following:

```
psql packagesite --file ./leaves.sql
```

You would need a database role for the SQL inquiry to function.
