
# FINGERTIPS

Final project for the Building AI course

## Summary

A mobile dating app that increases your probabilities of meeting matching people in real life by using user-provided data and location services.


## Background

According to a recent poll by YLE, Finland's national public broadcasting company, more than 50% of people meet their partner online, but only 10% regard it as the ideal way to meet someone. So 90% of people would prefer to meet someone in real life. In real life though, it's quite often difficult to figure out where you could meet the kind of people you might be interested in. This is where Fingertips comes in.

Fingertips is not an app for meeting people online. It's an app to motivate people to go out to the real world and meet people while being in places they like, doing things they like.

The difference between Fingertips and other dating apps is that in Fingertips, the user doesn't have a profile that would be visible to other users. Users can't see photos of each other, read about each other or contact each other through Fingertips. What Fingertips does is that it gives you a map to see where people that you match well are at the moment. It also gives you notifications, if someone you match really well with is near. In a way it's a bit like Pokemon GO for all us longing to meet someone interesting in real life.

I think it's interesting and desirable to try to develop solutions which make people engage more with each other in real life and which make us think human relationships as not something to optimize but as something to be open about and take a chance on. On personal level, as someone who doesn't like online dating, I have at times wondered where the heck all the intelligent, curious, kind-hearted guys spend their time. If this app would exist, I would love to use it.

The name fingertips comes from the expression “at fingertips”, meaning “being readily available”.




## How is it used?

In Fingertips, the user fills first in a detailed profile by answering to questionnaires and open questions about their interests and perspective on life and about the kind of person they are looking for. Then the user lets Fingertips track their whereabouts with location services so that data about their wherabouts can be used to tell other people in Fingertips where the user currently is. Because users don't have a public profile, other users will only see that someone fitting their interests is near. If the match is really good, Fingertips can send the user an optional notification that reads for example _1 person with whom you match with likelihood of 90 % or more is currently less than 100 m from you_. Fingertips will never give the real likelihood of match when it would be more than 90% because Fingertips is about giving yourself and the other a chance, not about optimizing your likelihoods.

Making contact with matches near them is up to the users. By just looking at the people around oneself, one can't know which one is a Fingertips match. Maybe one gather's their courage and talks to that interesting-seeming person on the bus stop, museum or grocery store, hoping that the person would be their match. Maybe it's not, but if it leads to something good, that's the most important thing, not that the person was your Fingertips match. And even though one would never try to find out who of the people around they are their matches, knowing that there are potential matches around makes life a bit more magical, doesn't it.

The user can define places that they want to exclude from the data, such as the area around their home, or work place where you don't want other users to locate you. They can also tag their current whereabouts, so that the notification that the potential match receives is more specific:_1 person with whom you match with 90% likelihood is currently in Kino Regina, less than 100m from you_.

By looking at the Fingertips map, you can easily go to places where the probabality of meeting matching people is high. Fingertips gives you also an optional weekly report about your probable matches, for example: _Last week you spent 3,8 hours less than 100m away from 5 persons with whom you have more than 80% match_. The proximity in metres and match percentage can be specified by user.



## Data sources and AI methods

The lure and usefulness of the app depends, besides an attractive and functional user interface, largely on getting quality data and processing it the way that it gives meaningful match results.

Data sources:
* Personal data about users and their preferences provided by users though questionnaires and open-ended questions 
* Data about users' location provided by the location service's on user's phone. 

AI techniques:
* For collecting data from questionnaires: linear regression, nearest neighbor method? 
* For collecting data from open-ended questions: TF-IDF, word2vec 
* For collecting data about user's location, excluding the areas on the map that each user wants to exclude: no AI needed but maybe it could be useful? 
* For combining the user's location with the user's preferences and calculating the probability that any two users would match and on which percentage they would match: optimization methods such as simulated annealing, neural networks? 

## Challenges

How people will become interested and motivated in using an app that doesn't give you direct, instant gratification but instead requires more action and even courage on your part?

How to analyze the user input so that it leads to quality data?

What is the treshold to how many users there needs to be for the app to function meaningfully?

Issues of privacy and the use of data: how to protect user's privacy and give them the simple enough but functional tools to adjust their own preferences regarding their privacy? How not to misuse any data, and how to give the user enough control over their own data?

Is the idea of your match being close to you motivational enough to find the courage to go to talk to someone you think might be your match?

...
## What next?

The idea behind this app, combining user-provided data to location services to find matching people, could be used also in other uses than dating, especially if it would be expanded to include future predictions of probability.

It can have more commercial applications, such as that any venue (e.g. club, museum, shop) could use it to draw in customers by promising them a higher than average probability of matches, or telling the customer at which hours and which days they have the high probabalility to meet people they match with (romantically, friend-wise, hobby-wise, etc.) It could also be used in social sciences for example in predicting how a new area of a city will be used and enjoyed by people, or in predicting occurrence of any other event or series of events in a specific location or locations, supposing that user input end user's location data can be collected.


