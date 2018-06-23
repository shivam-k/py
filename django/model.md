
Fields:
-------
Only required and v.imp

Fields options: 
--------------
null, blank, choices, deault, help_text, primary_key, unique

Relationships: 
--------------
### Many-to-one
use ```django.db.models.ForeignKey``` as a Field type
* ForeignKey requires a positional argument: the class to which the model is related.

### Many-to-many
use ```ManyToManyField``` as a Field type
* It doesn’t matter which model has the ManyToManyField (don't put in both)
* Name of the ManyToManyField be plural as suggested
* ``` a1.publications.add(p1)``` Associate the Article(a1) with a Publication(p1)
* ```new_publication = a2.publications.create(title='Highlights for Children')``` Create and add a Publication to an Article in one step using create()

### One-to-one
use ```OneToOneField``` as a Field Type