# Django-Database Models.py

Create a class with the name of your model.
Inherit the class from the `models.Model` class.

Then add fields like 'title', 'description', etc. (here)
Define these fields with methods from the `models` class.

Eg-
`title = models.CharField(max_length=200)`

To get the details of these fields just type the name of the field after (.) operator on the object of the model class.
`print(TaskObject.title)`

To learn more read the official documentation from https://docs.djangoproject.com/en/4.0/topics/db/models/
