django_location_choices
=======================

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
