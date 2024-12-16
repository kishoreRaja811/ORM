# Ex02 Django ORM Web Application
# Date:19/10/2024
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
admin.py:
from django.contrib import admin
from .models import bankloan,bankloanAdmin
admin.site.register(bankloan,bankloanAdmin

models.py:
from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    Name=models.CharField(max_length=100)
    Accountno=models.IntegerField(primary_key="Accountno")
    Startdate=models.DateField()
    Email=models.EmailField()
    Mobilenumber=models.IntegerField()
    Amount=models.IntegerField()

class bankloanAdmin(admin.ModelAdmin):
    list_display=('Name','Accountno','Startdate','Email','Mobilenumber','Amount')
```
# OUTPUT
![PAINT](https://github.com/user-attachments/assets/a789431a-8391-4a45-8059-d94088aca29a)
![Screenshot 2024-12-07 222431](https://github.com/user-attachments/assets/dece8314-36c1-48be-a5c6-1d3ca9dad98e)
![Screenshot 2024-12-07 222417](https://github.com/user-attachments/assets/67f7cf75-7a21-486a-aac0-19d9b3c476c1)
![Screenshot 2024-12-12 132041](https://github.com/user-attachments/assets/68f66a55-7821-4813-bbf9-0c5bc21ea3fd)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
