# MakersBnB
### Makers Academy Week No. 6

[![Build Status](https://travis-ci.org/KatHicks/makersbnb.svg?branch=master)](https://travis-ci.org/KatHicks/makersbnb) [![Coverage Status](https://coveralls.io/repos/github/KatHicks/makersbnb/badge.svg?branch=master)](https://coveralls.io/github/KatHicks/makersbnb?branch=master) [![Code Climate](https://codeclimate.com/github/KatHicks/makersbnb/badges/gpa.svg)](https://codeclimate.com/github/KatHicks/makersbnb)

**Built by [Mica Whitby](https://github.com/MicaW), [Kat Hicks](https://github.com/KatHicks), [Edyta Wrobel](https://github.com/edytawrobel) and [Mitch Goldbay](https://github.com/mbgimot) in 5 days at Makers Academy**

![Screenshot of landing page](/screenshot.png?raw=true "Screenshot of landing page")

### Instructions

> * You'll work in teams to build a clone of Airbnb
> * You'll organise your own work
> * We would like a web application that allows users to list spaces they have available, and to hire spaces for the night
> * Your coach will be around as usual

### User Stories

We were given a list of specifications and were required to develop user stories from them to guide our implementation. We also decided for ourselves what would be the minimum viable product (MVP).

**MVP**

```
As an owner,
So that rentees know about my space,
I can list a space with a name, price, and description.

As a rentee,
So that I only see information about properties of interest,
I can click on a space to see full details and make a booking.

As an owner,
So that I can rent multiple properties,
I can list multiple spaces.

As a rentee,
So that I can see where I want to stay,
I can view spaces listed on MakersBnB.

As a signed up rentee,
So that I can have a weekend away,
I can request a space for one night.
```

**Version 1**

```
As a user,
So that only I can make bookings,
I can log out of my account.

As an owner,
So that people don't book it when its not available,
I can list a space with available dates in one time window.

As a rentee,
So that I know whether the space is available during my chosen dates,
I can see the availability of a space.

As an owner,
So that I can respond to rental requests,
I can see the requests I have received for bookings.

As an owner,
So that I can retain control of my property,
I can approve a request for my space before it is booked.

As a rentee,
So that we don't have a duplicate booking,
I can't book somewhere that has already been booked.

As a user,
So that I know whether MakersBnB is for me,
I can view all the spaces available without logging in.

As an owner,
So that people don't book my space when its not available,
I can list a space with available dates in multiple time windows.

As an owner,
So that I can remind myself what I've listed on the site,
I can view spaces I have listed.

As a rentee,
So that I refer back to it if needed,
I can see the requests I have made for bookings.

As an owner,
So that I can retain control of my property,
I can deny a request for my space before it is booked.

As an owner,
So that I can choose who to rent my space to,
I can receive multiple requests to rent before I approve it.

As an owner,
So that I can ensure details are correct,
I can update a space I have listed.

As a signed up rentee,
So that I can have a holiday,
I can request a space for multiple nights.

As a MakersBnB manager,
So that I can persuade them to join MakersBnB,
I can display curated spaces to a user that hasn't logged in.

As an owner,
So that rentees know when to arrive and leave,
I can define the check in and check out times for my space.

As an owner,
So that more people look at it,
I want to add an image of my space.
```

### Objectives

* Are you having fun?
* Are you a better developer than you were yesterday?
* **Can you, with only a specification to guide you, work as part of a team to build a web app?**

### Using our app

* You can view our app at [cabinbnb.herokuapp.com](http://cabinbnb.herokuapp.com/)

### Running the tests

* If you do not have PostgreSQL installed, you will need to install it using the command `$ brew install postgresql`
* Enter the PostgreSQL console by typing `$ psql`
* Create two databases with the commands `$ create database makersbnb_test` and `$ create database makersbnb_development`
* Clone this repository using `$ git clone`
* Navigate into the directory using `$ cd makersbnb`
* Run `$ bundle` to install all the dependencies listed in the Gemfile
* **After all this setup is complete, you should be able to run the tests in the command line with `$ rspec`**

### Technologies

* Written using **Ruby 2.3.3** with **Sinatra** as the web framework
* Built off of a **PostgreSQL** database with **DataMapper** as the ORM
* Tested using **RSpec** and **Capybara**
  * Also used **Orderly** to test the order of content on the page
* Used the **BCrypt** gem for password encryption
* Deployed using **Heroku**

### Approach

* **Planning**
  * We spent the whole first day just on planning
  * Dedicated a lot of time to compiling all our user stories and mapping out our domain model
* **Reaching MVP**
  * Planning paid off and we reached MVP very quickly
* **Additional features**
  * After reaching MVP, the two sets of pairs dedicated themselves to two separate additional features
  * Additional features detailed below
* **Multiple date ranges**
  * One pair dedicated themselves to figuring out how to implement multiple date ranges for space availability
  * One of the simplifications of MVP was that spaces could be listed as available for one night only i.e. they were either available or unavailable
* **Image upload**
  * The other pair then dedicated themselves to implementing image upload when listing a space
  * We figured out how to do this after a days work without any assistance from external libraries or gems

### Ideas for extension

* **Finish styling**
  * Currently the styling is only half finished so it would be good to add to it
* **Email notification**
  * One of the nice-to-have specifications was integrating an API so that email notifications were sent after certain actions in the app - would be nice to implement this feature
