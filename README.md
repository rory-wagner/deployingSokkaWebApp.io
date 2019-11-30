# Avatar Quotes Web App

## Resource

**Characters**

Attributes:

* name (string)
* nation (string)
* quote (string)
* episode (integer)
* book (string)

**Users**

Attributes:

* First Name (string)
* Last Name (string)
* Username (string)
* Password (string)

## Schema

```sql
CREATE TABLE characters (
id INTEGER PRIMARY KEY,  
name TEXT,
nation TEXT,
quote TEXT,
episode INTEGER,
book TEXT);
CREATE TABLE users (
id INTEGER PRIMARY KEY,
firstName TEXT,
lastName TEXT,
userName TEXT,
password TEXT);
```

## REST Endpoints

Name                           | Method | Path
-------------------------------|--------|------------------
Retrieve character collection | GET    | /quotes
Retrieve character member     | GET    | /quotes/*\<id\>*
Create character member       | POST   | /quotes
Login user member             | POST   | /logins
Create user member            | POST   | /registrations
Update character member       | PUT    | /quotes/*\<id\>*
Delete character member       | DELETE | /quotes/*\<id\>*
