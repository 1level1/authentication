# authentication
Mobile (FE) and BE social authentication using React-Native and Django

This is a general example for authentication a of mobile app (FE), using third party (Facebook, Google...) and a BE service (Djange-Rest-Framework).

The highlevel flow is (App should already be registered, with an ap id):
1) Mobile App - user registers through 
Facebook SDK talks to Facebook backend to get a token
Your client gives your backend the token
Your backend validates the token against Facebook’s servers
Your backend issues a new authentication or session token
Your client saves your backend’s auth token: Now you’re logged in and can talk to your own servers forever, or at least in a way you understand.


## prerequisites:
1) 
