# Ex02 Django ORM Web Application
## Date:15/03/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![1](https://github.com/srinivasanvaiyali/ORM/assets/145117665/2873db48-7429-48a2-967f-3804d3d1a695)


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
```C
admin.py

from django.contrib import admin
from .models import book,bookAdmin
admin.site.register(book,bookAdmin)  

models.py

from django .db import models
from django.contrib import admin
class book(models.Model):
     book_no=models.IntegerField(primary_key=True)
     book_name=models.CharField(max_length=20)
     author_name=models.CharField(max_length=30)
     book_page=models.IntegerField()
     book_price=models.IntegerField()
     
class bookAdmin(admin.ModelAdmin):
    list_display=('book_no','book_name','author_name','book_page','book_price')
```

## OUTPUT
![2](https://github.com/srinivasanvaiyali/ORM/assets/145117665/7c24be72-8b10-4b15-bc94-946280126cfd)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
