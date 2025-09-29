# Ex02 Django ORM Web Application
# Date:29/09/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
from django.db import models
from django.contrib import admin
class Car_DB(models.Model):
    Brand_Name = models.CharField(max_length=10)
    Model_No = models.IntegerField(primary_key=True)
    Customer_name = models.CharField(max_length=10)
    Mfg_Date = models.DateField()
    Engine_type=models.CharField(max_length=10)
    Plate_Number=models.CharField(max_length=10)
class Car_DBAdmin(admin.ModelAdmin):
    list_display = ["Brand_Name","Model_No","Customer_name","Mfg_Date",'Engine_type'
                    ,'Plate_Number']

from django.contrib import admin
from.models import Car_DB,Car_DBAdmin
admin.site.register(Car_DB,Car_DBAdmin)

```
# OUTPUT
![alt text](<Screenshot (53).png>)
# RESULT
Thus the program for creating a database using ORM hass been executed successfully
