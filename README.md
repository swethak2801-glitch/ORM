# Ex02 Django ORM Web Application
# Date:23.09.2025
# AIM
To develop a Django application to store and retrieve data from Car Inventory database using Object Relational Mapping(ORM).

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
```
admin.py
from django.contrib import admin
from .models import CarInventory,CarAdmin

admin.site.register(CarInventory,CarAdmin)

models.py
from django.db import models
from django.contrib import admin
class CarInventory(models.Model):
    car_brand=models.CharField(max_length=20)
    car_model=models.CharField(max_length=20)
    mileage=models.IntegerField()
    engine_type=models.CharField(max_length=20)
    manfg_date=models.DateField()
class CarAdmin(admin.ModelAdmin):
    list_display=['car_brand','car_model','mileage','engine_type','manfg_date']

```

# Output
![alt text](<../Screenshot 2025-09-22 115352.png>)







# RESULT
Thus the program for creating a database using ORM hass been executed successfully
