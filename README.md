# Backend authentication using frontend (Mobile app) login

Mobile (FE) and BE social authentication using React-Native and Django

This is a general example for authentication a of mobile app (FE), using third party (Facebook, Google...) and a BE service (Djange-Rest-Framework). Will use google as an example, process is the same for all third party authenticatrion.


The highlevel flow is (App should already be registered, with an ap id):
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
4. Install PostgreSQL
5. Install react-native
