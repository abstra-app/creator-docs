# Microsoft SQL Server

![Configuration](../../../.gitbook/assets/screenshot_from_2021-04-26_16-08-55.png)

![Queries](../../../.gitbook/assets/image%20%2816%29.png)

You can write regular [SQL Server queries](https://www.sqlservertutorial.net/) here, for example:

```text
SELECT * FROM "Users" u WHERE u.name LIKE '%John%'
```

## Passing parameters to the query

You can add **params** to your query by naming them **$variable**. When you use this query in the frontend, you can dinamically fill the parameters:

```text
SELECT * FROM "Users" u WHERE u.name = $variable_name
```

Insert example:

```text
INSERT INTO "Users"(name, email) VALUES ($name,$email)
```

Update example:

```text
UPDATE "Users" SET name = $name WHERE u.email = $email
```

Delete example:

```text
DELETE FROM "Users" WHERE u.email = $email
```

