# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
A backend manages the database(s) and handles the interactions between the user
and the data.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
Model
```

Which layer in the MVC pattern communicates with the model?

```bash
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
We (standards) are moving towards SPA thus transferring the burden onto the client
```

What does C.R.U.D stand for?

```bash
Creat Read Update Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
Model
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
index, create, show, update, destroy
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
1. Browser sends GET request
2. Request passes through Route to Controller
3. Controller selects the corresponding Model and passes request
4. Model accesses DB, and executes request.
5. Request is now passed "down" the chain to the browser.
6. Views happen on a separate branch from the Controller
```

What is the command to generate a new rails-api app?

```bash
rails-api new name ...skip-stuff... --database=...
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
1. db:drop
2. db:migrate
3. db:create
```

What is the command to scaffold a pet with a name and an age?

```bash
rails-api g scaffold pet name:string age:fixnum
```

List two advantages of using serializers? (2 bullet points)

```bash
1. Automates creation of attributes (as objects)
2. Returns attribute as object thus increasing consistency
```
