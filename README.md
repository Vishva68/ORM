# Ex02 Django ORM Web Application
## Date:15/09/2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

<img width="1002" height="671" alt="image" src="https://github.com/user-attachments/assets/ff72a45a-d5d0-47a8-8ca6-00754ec902c3" />


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
```
from django.db import models
from django.contrib import admin
class  Movie_DB (models.Model):
    Movie_ID = models.CharField(max_length=20, primary_key=True)
    Title = models.CharField(max_length=100)
    Genre = models.CharField(max_length=20)
    Rating = models.IntegerField( )
    Language = models.CharField(max_length=15)
    Release_Date = models.DateField( )
class Movie_DBAdmin(admin.ModelAdmin):
     list_display = ('Movie_ID', 'Title', 'Genre', 'Rating', 'Language', 'Release_Date')
```

admin.py
```
from django.contrib import admin
from .models import Movie_DB, Movie_DBAdmin
admin.site.register(Movie_DB, Movie_DBAdmin)
```


## OUTPUT

<img width="1356" height="906" alt="Screenshot 2025-09-15 135552" src="https://github.com/user-attachments/assets/4c125d31-673e-4379-9604-3f76ba8a5b38" />




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
