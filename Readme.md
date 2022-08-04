# Django-Database Models.py

Models.py file stores the layout of how the data is stored in the database. It defines the columns o the database and the data types.

To start, we need to import the models module from the django.db package.

Create a class with the name of your model.
Inherit the class from the `models.Model` class.

Then add fields like 'title', 'description', etc. (here)
Define these fields with methods from the `models` class.

Eg-
`title = models.CharField(max_length=200)`

To get the details of these fields just type the name of the field after (.) operator on the object of the model class.
`print(TaskObject.title)`

The `models.ForeignKey` field is used to link the model to another model (`User` here). `User` is a predefined default model in Django for storing a user's data. ForeignKey is of the type `Many to One Relation`.

For example, in this case a user can have many tasks assigned to himself but a task cannot have multiple users assigned to it. Thus a user can have many tasks (Many to One Relation).

To learn more read the official documentation from https://docs.djangoproject.com/en/4.0/topics/db/models/
