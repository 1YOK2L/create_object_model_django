# How to create record models Author and Song

# class Author(models.Model):
#     name = models.CharField(max_length=255)
#     birth_date = models.DateTimeField()
#     class Gender(models.TextChoices):
#         MALE = 'M'
#         FEMALE = 'F'
#         UNKNOWN = 'N/A'
#     # GENDER_CHOICES = (
#     #     (Gender.UNKNOWN, 'N/A'),
#     #     (Gender.MALE, 'Male'),
#     #     (Gender.FEMALE, 'Female'),
#     # )
#     gender = models.CharField(choices=Gender.choices, default=Gender.UNKNOWN, max_length=6)
    
#     def __str__(self):
#         return self.name

from music.models import Author
from datetime import datetime
                                                         #yyyy, mm, dd, hh, mm, ss
Author.objects.create(name='Example', birth_date=datetime(2005,  2, 13,  2, 54,  0), gender='M')