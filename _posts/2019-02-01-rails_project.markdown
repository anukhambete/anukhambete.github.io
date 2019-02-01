---
layout: post
title:      "Rails Project"
date:       2019-02-01 17:41:43 +0000
permalink:  rails_project
---


My project is a simple Rails based application that allows users create itineraries of their stays in New York city or suggest itineraries in the city.

The aim of the site is to provide users the chance to access suggested itineraries listed by other people, list their own itineraries based on their experiences and share and like tips about their activities. 

The models that were created were:
* 1)	User Model
* 2)	Itinerary Model
* 3)	Place Model
* 4)	Likes Model

Each user registers a valid username, email and password. Users can also login into the app via facebook. In order to ensure that there’s no conflict with the facebook login details the site requires that each new user have a unique email address.

The users can perform all the CRUD actions on the itineraries that were created by them. Each itinerary, belongs to a user and must be initialized with a name and description. A single user can create multiple itineraries. Ideally the description should contain a brief description or review of the places that were visited/listed on that itinerary.

A number of places can be added to the itinerary by the user of that itinerary. The place/ site visited contains the name and the borough in which it resides. For simplicity a user cannot add multiple locations with the same name in the same borough. Each itinerary contains a unique list of places/sites to visit. The users can have many places through itineraries and vice versa.
The users are allowed to add as many places as they wish or delete them but only as part of their itineraries. They cannot edit the name or the borough of the place, only remove it from the list and add the correct entry.

The users can also like itineraries created by others. They have the option of liking and subsequently removing the likes if they change their minds. Likes belong to both users and itineraries

The site also has an ‘admin’ user that has access to create and delete certain records that regular users do not have access to. The site admin can create places/sites to add to the Index of Places as well as edit the name and borough. For example, if a user accidentally lists the Empire State Building as part of Queens, only the site admin has the rights to edit the place and change the borough to Manhattan.

