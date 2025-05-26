# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![Screenshot 2025-05-09 110412](https://github.com/user-attachments/assets/6b07e9e6-5b03-4969-b463-b42960e564bc)


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
from django.contrib import admin
class loan (models.Model):
    Loan_Id=models.CharField(max_length=20,primary_key=True)
    Name=models.CharField(max_length=100)
    Age=models.IntegerField()
    Salary=models.IntegerField()
    Loan_applied_date=models.DateField()
    Loan_amount=models.IntegerField()
    Email=models.EmailField()
    Phone_no=models.IntegerField()


class loanAdmin(admin.ModelAdmin):
    list_display=('Loan_Id','Name','Age','Salary','Loan_applied_date','Loan_amount','Email','Phone_no')


admin.py
from django.contrib import admin
from .models import loan,loanAdmin
admin.site.register(loan,loanAdmin)



## OUTPUT
![Screenshot 2025-05-09 110350](https://github.com/user-attachments/assets/d0fc469e-7f49-44bd-8f64-230b24f60290)

![Screenshot 2025-05-09 110402](https://github.com/user-attachments/assets/3cb522a3-6685-4000-b210-f906bec0ef93)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
