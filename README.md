# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![eremp_11zon](https://user-images.githubusercontent.com/120367796/230323793-8e2e4813-354e-41dd-a1a1-65abf47f7386.jpg)


## DESIGN STEPS

### STEP 1:
Clone the problem from the github

### STEP 2:
Create a new app

### STEP 3:
Enter the code for admin.py and model.py

### STEP 4:
Execute Django admin and create 10 employees

## PROGRAM
```
Admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

Model.py

from django.db import models
from django.contrib import admin
class Employee (models.Model): 
    eid=models.CharField(max_length=20, help_text="Employee ID") 
    name=models.CharField(max_length=100) 
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models. EmailField()

class EmployeeAdmin (admin. ModelAdmin):
    list_display=('eid','name','salary','age','email')

```


## OUTPUT

 ## SERVER OUTPUT:
![jango server](https://user-images.githubusercontent.com/120367796/233534340-9a6322d5-0dbe-4170-921f-9a9b4e7882df.png)

 
 ## CLIENT OUTPUT:
![employee](https://user-images.githubusercontent.com/120367796/230316980-b245e447-d560-4545-b8b8-746f42360604.jpg)
 


## RESULT

The  code executed successfully
