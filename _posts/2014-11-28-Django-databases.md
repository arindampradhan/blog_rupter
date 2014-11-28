---
layout: post
title: Django databases
location: Bhubaneswar
tags:
- places
---


I have been looking into django for a while,some opensource organization use django a lot.
Some of the cool features I found about django is 
the extensions module django-extensions.

It really gives some cools features.

To install it :

	pip install django-extensions

	or to get the latest release

	git clone git://github.com/django-extensions/django-extensions.git
	cd django-extensions 
	python setup.py install


The cool feature I came across while playing django-extensions is shell_plus

>Shell_plus is a management command provided by the django_extensions app. It gives you everything that shell gives you, but it also automatically imports all of your models from all of your installed apps. This can be a very nice shortcut when your experimenting with model code.

It can give a much more useful output! We can get an idea of which object each entry in the query set represents. 

Few common tricks which we use with models 
are :
	from django.db import models
	from django.contrib.localflavor.us.models import PhoneNumberField

	class Library(models.Model):
		name = models.CharField(max_length=200)
		phone_number = PhoneNumberField()


		def __unicode__(self):
			return self.name


## __unicode__
__unicode__ is like the default __repr__ in django

always defining a __unicode__ is healthy shortcut for playing with databases cause when we play with them we can easily see their representation.




Cool now lets headstart for database:
	./manage syncdb (synchronize the db)

	./manage shell_plus

It will automatically load the models for you to play with.
	
	>>> lib = Library(name="New York Public Library",phone_number='212-222-6559')
	>>> lib.save()

Dont use this method while in prompt 

	>>> lib = Library.objects.create(name="New York Public Library",phone_number='212-222-6559')
	>>>	lib2 = Library.objects.create(name='Seaford Public Library', address='2234 Jackson Ave', state='NY', zip_code='11783', phone_number='516-221-1334')

You wont need to save them again and again to avoid conflicts.

	>>> Library.objects.all()

To show the objects



##SOME COOL METHOD 
	
>not **get** but **get_or_create**

As the name suggests it will try to find an object with the parameters you provide and if it cannot find one, it will create one.

> use **filter** instead of **get**

Simply cause it's easy to use and give two awesome parameters :
* *__startswith*
* *__contains*

	>>> Library.objects.filter(state='NY')
	[<Library: New York Public Library>, <Library: Seaford Public Library>]
	>>> Library.objects.filter(**name__startswith**='Public')
	[<Library: Public Library of Princeton>]
	>>> Library.objects.filter(**name__contains**='c')
	[<Library: New York Public Library>, <Library: Seaford Public Library>]

Just append them to the query parameter string.


**Delete** and **Update** are pretty simple.You just catch the elements with get or filter and delete them or update them cool.
Soon I will talk about them and relational database about **one to one** and **many to many**. 
That's up for today's enjoyment...!!
My sems are tomorrow...:P So ,BYE