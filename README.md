# Ex02 Django ORM Web Application
## Date: 25-11-2025
## Ref no: 25012095

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).


## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code of admin.py and models.py


### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
~~~~
admin.py 

from django.contrib import admin
from .models import amazon_DB,amazon_DBAdmin
admin.site.register(amazon_DB,amazon_DBAdmin)

models.py

from django.db import models 
from django.contrib import admin
class amazon_DB (models.Model):
     Product_name=models.CharField(max_length=20)
     S_no=models.IntegerField (primary_key=True)
     Product_type=models.CharField(max_length=20)
     Price=models.CharField(max_length=20)
     Year=models.IntegerField()
class amazon_DBAdmin(admin.ModelAdmin):
     list_display=["Product_name","S_no","Product_type","Price","Year"]

~~~~



## OUTPUT

![shree](https://github.com/user-attachments/assets/5aae350e-948d-498b-9b24-fd542f08c81b)

![shree 1](https://github.com/user-attachments/assets/d66ce8db-5ff4-44d6-8dd7-4726534b78b1)


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
