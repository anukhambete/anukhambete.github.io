---
layout: post
title:      "Sinatra Project"
date:       2018-10-31 17:54:15 +0000
permalink:  sinatra_project
---


Selecting the Sinatra project was governed by two main factors. First, was the condition to have one has many, belongs to relationship between two models and then implement an additional has many relationship. Second, was the need to think of scenarios where one user can view another user’s content but not have the ability to edit or delete it.

The Labs covered instances of users being able to perform CRUD actions on posts which belonged to them. This only involved two models, where the users had many posts and each post belonged to a user. 
* The example I’ve chosen thinks of the user as a singer or a band. Each user can have many albums and each album in turn can have many songs. 
* The albums table lists the name and year of release as its attributes whereas the song table lists the song name and the track length. 
* Each user/artist can create and album and add songs to it or begin by creating a song and declaring the album name while creating it.
* The user i.e. the creator of the album/song should have the ability to edit the album and the songs contained in it provided the album belongs to the user. The users can only view the albums and songs of other users without being able to edit or delete them.

The most challenging part of the project was accounting for errors while editing or creating a new album/song. I incorporated some logic to ensure that the user was not creating the same album or song twice.
I had some unexpected errors when I tried to use the album_controller and then came across another student blog that dealt with naming conventions and how it may clash with the Application controller. Appending the album_controller with ex or with any other combination of letters that doesn't being with 'a' seemed to solve the problem.
