---
id: 917
title: Thursday Football
date: 2014-03-11T19:04:12+00:00
author: Simon Barnett
guid: http://www.acresofspace.co.uk/?page_id=917
slide_template:
  - ""
---
[pullquote style=&#8221;right&#8221;]A simple way to organise a weekly 5-a-side football match[/pullquote]  
_A Django-based website which is used to manage a weekly 5-a-side football match. The site is deployed on Heroku and features automated player selection (using a rolling, points-based system), interactive team selection, form tables, player stats and regular email reminders._

[clear]

#### Beginnings

[two_third]

The Thursday Football website was born out of my desire to automate the organisation of my weekly game of 5-a-side football.

This laborious process had always been done with a combination of some _very_ complicated spreadsheets and _lots_ of emails.

There were a lot of problems with the old system. Firstly, the spreadsheets were too complex and no-one ever bothered to check to see how much they owed or whether they were playing. This meant that I had to spend a lot of time chasing people for money and sending out emails to check that everyone could play.

It was also easy for people&#8217;s emails to get lost and for us to find ourselves with either 9 or 11 players on a match day. Furthermore, there were endless arguments about who should and shouldn&#8217;t be playing.

Something had to be done.

[/two_third]

[one\_third\_last]  
[shashin type=&#8221;photo&#8221; id=&#8221;5756&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one\_third\_last]

[clear]

#### What Do Points Make?

We&#8217;d operated a points-based system for some time. Players earned points for playing and, using a sliding window of the last 10 games, the top 10 scorers would be asked whether they wanted to play each week. This naturally lent itself well to using a web framework such as Django.

I&#8217;d been doing some work with Python in my working life and had written a very basic web application to manage our weekly cake-baking rota () so I put my spare-time mind to learning more about Django and putting together a &#8220;proper&#8221; site, using Twitter Bootstrap for the UI and some JQuery for some user interactions.

#### Results

The site has now been up and running for a few months (March 2014) and has been working very well. It has dramatically reduced the amount of time any of us spend on administration and I&#8217;ve been able to easily recoup financial losses from people who can now easily see their debts via the site.

I have even added form tables and a points penalty system for those that continue to owe me money. I have plans to add automated team choosing &#8211; based on the data we are collecting &#8211; to the site, as well as other analysis on each player&#8217;s results and other statistics. The site has also inspired some of the other players and I have had many suggestions of things I could add to it.  
[one_half]

#### Login

This is the current login page. I had some problems with Django registration when using custom user models so for now I just ask people to email me if they want to play.

[/one_half]

[one\_half\_last]  
[shashin type=&#8221;photo&#8221; id=&#8221;5754&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one\_half\_last]

[one_half]  
[shashin type=&#8221;photo&#8221; id=&#8221;5752&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one_half]

[one\_half\_last]

#### Logged In

Once successfully logged in, the user arrives at the home page. Here, you are able to select your availability for the next game as well as being shown some useful player statistics.

[/one\_half\_last]

[one_half]

#### Logged In &#8211; Future Games

The user is also able to select their availability for future games from the home page.

[/one_half]

[one\_half\_last]  
[shashin type=&#8221;photo&#8221; id=&#8221;5755&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one\_half\_last]

[one_half]  
[shashin type=&#8221;photo&#8221; id=&#8221;5759&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one_half]

[one\_half\_last]

#### Choosing Teams

Once there are enough players to play a game, random team chooser is selected. This player is then able to select the teams for the game by dragging and dropping each player into a team.

[/one\_half\_last]

[one_half]

#### Teams Chosen

Once all the players have been assigned a team, the team chooser submits the teams and an email is sent to each player showing them who is playing on which team.

[/one_half]

[one\_half\_last]  
[shashin type=&#8221;photo&#8221; id=&#8221;5760&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one\_half\_last]

[one_half]  
[shashin type=&#8221;photo&#8221; id=&#8221;5762&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one_half]

[one\_half\_last]

#### Results

The application includes a page which lists all of the previous results along with (optionally) the players that played on each team. Each player also has their own individual page which lists only the games that they played in as well as a &#8220;finances&#8221; page which shows their payments as well as games played.

[/one\_half\_last]

[one_half]

#### Players

This page shows all of the players, along with their current score and a list of the last 10 games and whether they played, were a substitute or were not available. For the admin users, this page also shows how much money each player owes (or is in credit).

[/one_half]

[one\_half\_last]  
[shashin type=&#8221;photo&#8221; id=&#8221;5761&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one\_half\_last]

[one_half]  
[shashin type=&#8221;photo&#8221; id=&#8221;5758&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one_half]

[one\_half\_last]

#### Form

We calculate a form table, based on an averaged points per game played so we can aid players in selecting the teams each week in order to try and make the game competitive.

[/one\_half\_last]

[one_half]

#### Game Details

There is also a page which shows the location of the pitch and some rules of the game.

[/one_half]

[one\_half\_last]  
[shashin type=&#8221;photo&#8221; id=&#8221;5757&#8243; size=&#8221;medium&#8221; columns=&#8221;max&#8221; order=&#8221;user&#8221; position=&#8221;center&#8221;]  
[/one\_half\_last]
