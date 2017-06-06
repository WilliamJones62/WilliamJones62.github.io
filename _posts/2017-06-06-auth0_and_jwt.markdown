---
layout: post
title:  "Auth0 and JWT"
date:   2017-06-06 00:54:56 +0000
---


Auth0 provides single sign on and token based authentication for one of my Angular JS front end applications. Auth0 uses JSON Web Tokens (JWT) in the authentication process. I have a Ruby on Rails backend API. What I needed was to pass the user ID to the backend so that the user could only update and delete data from the database that they had created. Auth0 provides a JWT decoder that breaks down the JWT into it's constituent parts. The part that contains the user id is called the sub claim (decoded.sub) of the JWT payload. This is what is passed to the server and stored on all data created by the user.

The tricky part is that there are 2 JWTs created by Auth0, the Access token and the ID token. Apparently access tokens aren't supposed to be decoded and read in client side applications, so the ID token is the one to use.
