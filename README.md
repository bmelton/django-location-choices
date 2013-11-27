django_location_choices
=======================

A simple collection of tuples for COUNTRY and STATE listings, for use in Django
projects that will offer state and country choices. 

In short, I just got tired of having to find this list every time I needed it, 
so it was easier to just package it up as a pip installable package than to 
keep futzing around with it every time. 

This is the possibly the smallest open source package ever, so I just went ahead
and made it a version 1.0.0 (and then found multiple small errors with setup.py
and README, causing me to delete the package over and over again to keep it at 1.0). 

The comments for this package now exceed the amount of source code, so I'm gonna 
shut up.  However, forks & pulls are welcomed. 

Installation
===

`pip install django_location_choices`

Usage
===

`from django_location_choices.locations import COUNTRY_CHOICES, STATE_CHOICES`

In your models, just reference those values for your CHOICES fields. 

```
class Thing(models.Model):
    state               = models.CharField(max_length=100, choices=STATE_CHOICES)
    country             = models.CharField(max_length=100, choices=COUNTRY_CHOICES)
```
