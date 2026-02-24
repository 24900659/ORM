# Ex02 Django ORM Web Application
## Date: 6.02.26

## AIM
To develop a Django application to manage an online food delivery platform like Zomato/Swiggy using Object Relational Mapping (ORM).

## ENTITY RELATIONSHIP DIAGRAM
<img width="519" height="774" alt="Screenshot (500)" src="https://github.com/user-attachments/assets/a5ef5d9d-5039-48f1-99d4-2d01d5d026cc" />





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
class Employee(models.Model):
    OrderID = models.IntegerField(primary_key=True)
    UserID = models.CharField(max_length=100)
    OrderDate = models.DateField()
    ItemName = models.CharField()
    OrderQty =models.IntegerField()
    UnitPrice = models.FloatField()
    TotalAmount = models.FloatField()
    DeliveryAddress = models.CharField()

class EmployeeAdmin(admin.ModelAdmin): 
        list_display=( 'OrderID','UserID','OrderDate','ItemName','OrderQty','UnitPrice','TotalAmount','DeliveryAddress')

```



## OUTPUT
<img width="1920" height="1080" alt="Screenshot (442)" src="https://github.com/user-attachments/assets/46d8dd4b-a77d-459b-8492-ebce5dd0f38d" />



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
