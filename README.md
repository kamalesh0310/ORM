# Ex02 Django ORM Web Application
## Date: 27.11.2025
ref no:25018201

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).


## ENTITY RELATIONSHIP DIAGRAM



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
~~~
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

admin.py

from django.contrib import admin
from .models import amazon_DB,amazon_DBAdmin
admin.site.register(amazon_DB,amazon_DBAdmin)
~~~

## OUTPUT
![WhatsApp Image 2025-11-27 at 22 14 22_a97a3ab1](https://github.com/user-attachments/assets/35fafc6b-fc6a-421d-9d17-1f9aaf2e1b08)
![WhatsApp Image 2025-11-27 at 22 14 24_f3a596ff](https://github.com/user-attachments/assets/959348b4-0a72-4013-ba13-339c48962b2d)


Include the screenshot of your admin page.


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
