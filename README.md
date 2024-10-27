# Ex02 Django ORM Web Application
## Date: 27/10/2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![alt text](<Screenshot 2024-10-27 101931.png>)


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
```


from django.db import models
from django.contrib import admin
class BankLoan(models.Model):
 Bln=models.CharField(max_length=20,primary_key="Bln")
 name=models.CharField(max_length=100)
 Loanamount=models.IntegerField()
 address=models.CharField(max_length=100)
 age=models.IntegerField()
 phoneno=models.IntegerField()

class BankLoanAdmin(admin.ModelAdmin):
 list_display=('Bln','name','Loanamount','address','age','phoneno')


```


## OUTPUT
[text](README.md) ![text](<Screenshot (5).png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
