# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).


## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
models.py
---------
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
admin.py
----------
from django.contrib import admin
from .models import amazon_DB,amazon_DBAdmin
admin.site.register(amazon_DB,amazon_DBAdmin)

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM


<img width="1920" height="1020" alt="Screenshot 2025-11-22 161056" src="https://github.com/user-attachments/assets/f656df5d-2ea1-47f7-bb17-3c8ea6e49a66" />

## OUTPUT

Include the screenshot of your admin page.

![WhatsApp Image 2025-11-23 at 19 58 35_20b53880](https://github.com/user-attachments/assets/dcf6aab5-4927-4223-8ba6-ae15dbe2b35b)

## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
