# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
The backend allows you to save data and access that data.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The model.
```

Which layer in the MVC pattern communicates with the model?

```bash
The controller.
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Our version of a view is the JSON that we will be passing to the front end. We
don''t use the views provided because there are front ends which will display
what we want better than the provided views.
```

What does C.R.U.D stand for?

```bash
C = create
R = read
U = update
D = destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
The controller.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```bash
get => index => show all
get => show => show one that is specified
post => create => make something new
patch => update => change this thing that i''ve specified, as i''ve specified
delete => destroy => delete this thing that i''ve specified

```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
*goes to the routes
*goes to controller
*goes to controller action
*goes to model
*goes to database
*goes to model
*goes to controller
*goes back to client
```

What is the command to generate a new rails-api app?

```bash
rails new rails-api (assuming that the name of the app that you want to create is
rails-api)

```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
```

What are the commands to drop, create and migrate a database from the command
line? (3 bullet points)

```bash
* bundle exec rails create (name of the database)
* bundle exec rake db:migrate
* bundle exec rails destroy (name of the database)

```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate scaffold pet name:string age:integer
```
