# Ex02 Django ORM Web Application
## Date: 04-04-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![WhatsApp Image 2024-04-04 at 21 00 44_5475bf33](https://github.com/23012925/ORM/assets/150931013/ed3fa707-4cf5-415a-beb3-f7c5195117e8)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM

```
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models

from django.contrib import admin

class Employee (models.Model):
    eid=models.CharField(max_length=20, help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid', 'name', 'salary', 'age', 'email')

```

## OUTPUT

![Screenshot 2024-04-04 155454](https://github.com/23012925/ORM/assets/150931013/593118b9-5bba-427d-84b2-09236a838bbc)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
