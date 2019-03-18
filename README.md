# Backend authentication using frontend (Mobile app) login

Mobile (FE) and BE social authentication using React-Native, Django and PostgreSQL

This is a general example for authentication a of mobile app (FE), using third party (Facebook, Google...) and a BE service (Djange-Rest-Framework). Will use google as an example, process is the same for all third party authenticatrion.


The highlevel flow is (App should already be registered - have app id):
1) Mobile App - user login to third party
2) Third party supplies a token
3) Pass token to BE
4) BE validates the token with third party, retrieves requested data.
5) BE supplies a new token for session.
6) App, user, uses token for communicating with backend API.

## Instalation:
1. Python >= 3.6
2. virtual env:
    1. python.exe -m venv /venv/path
    2. source /venv/path/Scripts/activate
3. Install Django, Django-Rest-Famework
    1. pip install django
    2. pip install django-rest-framework
4. Install PostgreSQL
5. Install react-native

## Implementation:
### Backend app - Simple django REST app:
The examples are based on the following links:

https://www.django-rest-framework.org/tutorial/4-authentication-and-permissions/

https://www.django-rest-framework.org/api-guide/authentication/

The basic step for almost all apps is to create a user. 

Luckily Django rest framework (drf) already supports such requirement.

1. Create a simple django app


