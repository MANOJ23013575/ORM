# Ex02 Django ORM Web Application
## Date:13.03.2024

## AIM
To develop a Django application to store and retrieve data from a railway database using Object Relational Mapping(ORM).
## Entity Relationalship Diagram
![WhatsApp Image 2024-03-19 at 16 02 59_04c3c670](https://github.com/MANOJ23013575/ORM/assets/159795359/97df97b0-ba02-4e85-a3d2-eb996caf4b75)
## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 records

## PROGRAM
'''
admin.py

from django.contrib import admin
from .models import railway,railwayAdmin
admin.site.register(railway,railwayAdmin)

models.py

from django.db import models
from django.contrib import admin
class railway (models.Model):
    train_code=models.CharField(max_length=20,help_text="railway train_code")
    train_name=models.CharField(max_length=100)
    start_time=models.IntegerField()
    End_time=models.IntegerField()
    start_station_code=models.IntegerField()
    end_station_code=models.IntegerField()
    
 
class railwayAdmin(admin.ModelAdmin):
    list_display=('train_code','train_name','start_time','End_time','start_station_code','end_station_code',)

'''

## OUTPUT

![alt text](<Screenshot 2024-03-13 194131.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
