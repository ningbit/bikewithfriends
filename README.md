#Bike With Friends! [@BikeWithFriends](http://twitter.com/bikewithfriends)
Gamify CitiBike

![BikeWithFriends](http://ningbit.github.io/images/bwf-stats.png)

#### Team Members:
- Ning Yap - [@ningbit](http://twitter.com/ningbit)
- Anisha Vasadani - [@foodismynish](http://twitter.com/foodismynish)
- Joshua Collins - [@jcalebcollins](http://twitter.com/jcalebcollins)
- Katie Ishibashi - [@floggingkatie](http://twitter.com/floggingkatie)

## Intro
BikeWithFriends is a social, interactive app that adds to the CitiBike experience by adding friend interactions, leaderboards, badges, trip histories, and more!
BikeWithFriends employs Ruby on Rails, the mechanize gem, CitiBike member trip data, CitiBike JSON station data, and Google Maps API.

## Notes on running the app

###Check out db/migrate/seeds.rb
- It runs several methods that seed data saved to lib/assets

###Login page:
- Leave the password field blank to login as a seeded user, just use their username.
- Username can be determined by looking at lib/assets: [username]_profile.html and [username]_trips.html

###How to add yourself and other users
- Login with your citibike username and citibike password, it will scrape the site and award you badges, check the Create method in Users Controller to see what happens
*or*
- Save and put your Profile and Trips .html files into lib/assets, taking care to name it following the conventions of "[username]\_profile.html" and "[username]\_trips.html"
- Edit app/models/seedable.rb

````
      def seed_data
        seed([your_username])
      end
````
      
- Run rake db:reset

## Screenshots

![BikeWithFriends](http://ningbit.github.io/images/bwf-maps.png)

## Events

#### We've been selected as "Hack of The Month" for NY Tech Meetup! We'll present
- On: Wednesday, August 7th, 2013
- At: NYU Skirball Center For The Performing Arts, 566 Laguardia Place

## Past Events

#### CitiBike / #BikeNYC Hacknight #2 for #betaNYC/Code For America

- On: Wednesday, July 31st, 2013
- At: NYU Wagner, The Puck Building, 295 Lafayette St, NYC

#### NYC on Rails Meetup @ The Flatiron School

- On: Thursday, July 25th, 2013
- At: 33 West 26th Street
