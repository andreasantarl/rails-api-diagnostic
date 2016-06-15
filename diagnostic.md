# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
The backend allows you to run calculations, make server requests, etc without disturbing the user interface
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
the model
```

Which layer in the MVC pattern communicates with the model?

```bash
The controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Everything needs to go through the controller
```

What does C.R.U.D stand for?

```bash
Create
Read
Update
Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
The model
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
SELECT, UPDATE, DELETE, POST, PATCH
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
-The user submits information into the application through the view
- the controller takes that information and triages it appropriately throughout the model.
- The model then runs any actions required (like updating data, running calculations, etc), and
- then the model sends it back to the view once the request is completed.
```

What is the command to generate a new rails-api app?

```bash
rails-api new movies_app -T --database=postgresql
```

What is the command to start an instance of a rails server?

```bash
rails s
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
$ bin/rake db:drop
$ bin/rake db:create
$ bin/rake db:migrate
```

What is the command to scaffold a pet with a name and an age?

```bash
$ bin/rails generate scaffold Pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
- Serializers allow you to use your data like an ActiveRecord object.
- If you need to update something, it will update all instances that have been used with that
serializer.
```
