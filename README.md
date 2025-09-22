# Ex02 Django ORM Web Application
## Date: 19/09/2025

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

<img width="940" height="506" alt="image" src="https://github.com/user-attachments/assets/f3f94aa0-fb3e-48ba-ab66-a101308fb2af" />


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
models.py
from django.db import models
class car(models.Model):
    car_id=models.IntegerField(primary_key=True)
    brand=models.CharField(max_length=30)
    model=models.CharField(max_length=30)
    year=models.DateField()
    price=models.IntegerField()

admin.py
from django.contrib import admin
from .models import car
admin.site.register(car)
class caradmin(admin.ModelAdmin):
    list_display=('car_id','brand','model','year','price')


## OUTPUT

![alt text](EXP2.png)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
