# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Screenshot 2023-04-16 003501](https://user-images.githubusercontent.com/112475766/232248788-16ed06ef-0e7d-4944-94cc-9bc1c3f48618.png)


## DESIGN STEPS

### STEP 1:
An Django application is created inside dataproject folder.

### STEP 2:
A python program is written to create a table to store and retrieve data.

### STEP 3:
The table is created with 6 fields in which the username field is made as PrimaryKey.

### STEP 4:
Then the project files migrated. A superuser is also created.

### STEP 5:
Now the server side program is executed .

### STEP 6:
The admin page of our website is accessed using username and password.

### STEP 7:
Records are added and saved in the table inside the database.

Write your own steps

## PROGRAM

```python
from django.db import models
from django.contrib import admin
# Create your models here.
class StudentMaster(models.Model):
    register_number = models.CharField(max_length=8, primary_key=True ,help_text="register_number")
    studentname = models.CharField(max_length=10)
    course = models.CharField(max_length=20)
    phone = models.IntegerField()
    email = models.EmailField()
    address = models.CharField(max_length=100)
class StudentMasterAdmin(admin.ModelAdmin):
    list_display = ('register_number','studentname','course','phone','email','address')

```

## OUTPUT
![Screenshot 2023-04-16 002828](https://user-images.githubusercontent.com/112475766/232248587-d6aa3bf2-ae3c-4574-835a-aba7145489f8.png)


## RESULT

Thus a Django application is successfully developed to store and retrieve data from a database using Object Relational Mapping(ORM).
