# Ex02 Django ORM Web Application
## Date:22.10.2025
## 25018961

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
rom django.db import models 
from django.contrib import admin
class amazon_DB (models.Model):
     Product_name=models.CharField(max_length=20)
     S_no=models.IntegerField (primary_key=True)
     Product_type=models.CharField(max_length=20)
     Price=models.CharField(max_length=20)
     Year=models.IntegerField()
class amazon_DBAdmin(admin.ModelAdmin):
     list_display=["Product_name","S_no","Product_type","Price","Year"]
~~~

~~~
admin.py
rom django.contrib import admin
from .models import amazon_DB,amazon_DBAdmin
admin.site.register(amazon_DB,amazon_DBAdmin)
~~~


## OUTPUT
<img width="1919" height="1079" alt="Screenshot 2025-11-21 153530" src="https://github.com/user-attachments/assets/15e543a3-9022-4685-97dd-ee3f3f806450" />
<img width="1077" height="866" alt="Screenshot 2025-11-21 153620" src="https://github.com/user-attachments/assets/9527cb30-e8be-4984-8311-cf96738c38e0" />

Include the screenshot of your admin page.


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
