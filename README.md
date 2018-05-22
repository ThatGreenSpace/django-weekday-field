# django-weekday-field

Weekday field for Django

This project has been created rather than forked because there has not been any proper ownership of this project either on Github or Bitbucket. It was first on Github and then it was moved to Bitbucket and then another person has a copy of this on Github. None of these repos match the code on PyPi

So rather than forking, this project is a copy of the PyPi version.

It has been modified to support Django 1.10.


# TODO
This codebase doesn't support Django 2.0 and above and hence needs to modified to do so.


## Description
A field that encapsulates the handling of selection of 0 or more weekday choices.

Uses Django's CommaSeparatedIntegerField internally.

Usage:

    from django.db import models

    import weekday_field

    class MyModel(models.Model):
        weekdays = weekday_field.fields.WeekdayField()
