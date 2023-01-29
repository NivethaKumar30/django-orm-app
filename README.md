# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram


## DESIGN STEPS

STEP 1:
Create a new Django project using "django-admin startproject",get into the project's terminal and use "python3 manage.py startapp" command.

STEP 2:
Define a model for the BankAccountmembership in the models.py and allow host access and add the app name under the installed apps in settings.py

STEP 3:
Register the models with the Django admin site. In admin.py under app folder, register the models with Django admin site

## PROGRAM
from django.db import models

# Create your models here. 
from django.db import models
from django.contrib import admin
# Create your models here.
class Customer(models.Model):
    customerid = models.CharField(max_length=8,primary_key=True)
    customername =models.CharField(max_length=100)
    mobilenumber =models.CharField(max_length=100)
    email = models.EmailField()
    quantity= models.IntegerField()
    

class CustomerAdmin(admin.ModelAdmin):
    list_display = ('customerid','customername','mobilenumber','email','quantity')

## OUTPUT

## RESULT
Thus a Django application to store and retrieve data from a database using Object Relational Mapping(ORM) is developed
