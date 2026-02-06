# Ex02 Django ORM Web Application
## Date: 6.02.26

## AIM
To develop a Django application to manage an online food delivery platform like Zomato/Swiggy using Object Relational Mapping (ORM).

## ENTITY RELATIONSHIP DIAGRAM
<img width="1691" height="794" alt="Screenshot (430)" src="https://github.com/user-attachments/assets/9184d8c9-bdd9-49db-a17b-e27b1d227689" />




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
from .models import Employee, EmployeeAdmin
admin.site.register(Employee, EmployeeAdmin)

models.py
from django.db import models
from django.contrib import admin

class Employee(models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')



## OUTPUT
<img width="1920" height="1080" alt="Screenshot (427)" src="https://github.com/user-attachments/assets/c559250d-6513-43b0-9857-a0dcbe784cd4" />


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
