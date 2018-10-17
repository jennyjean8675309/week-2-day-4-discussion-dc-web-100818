# Domain Modelling Discussion Questions

### Discuss these questions with your fellow table mates and try to model some solutions to the questions  


##### Using Netflix as your model, think about/try to model some solutions for the following questions:

1 . What would a Users table look like? What columns do you think would be in the table?

User id as a primary key, user name (first and last), icon

2 . As a user you should be able to look at a list of movies and select any individual movies to add to your Queue. How would you model the relationship between a User and their Queue of Movies? What kind of properties would a Queue have? What kind of relationships would a Queue have with other tables? _Be sure to be very clear about on which table(s) the foreign keys are found. Be sure your domain allows the same Movie to appear on many different user's queues_

User has many movies, movies can have many users, join table would have users and movies (joined by user id and movie id)/each instance of a queue's user and queue's movie would belong to just one user and one movie

3 . A Movie has a plot, title, rating, duration, actors/actresses, and reviews. How would you model each of these relationships with a Movie. What would would you call the relationship between an Actor and a Movie?

Plot, title, duration would belong to one movie, one movie has many ratings and reviews, each instance of rating/review would belong to only one movie, one movie would have many actors/actresses, and actors/actresses can have many movies so you would need a join table for that relationship, actors/actresses can have many reviews through movies

4 . As a user you should be able to leave a Review on a Movie. Would a Review be a property of a User or it's own table? Why? If a Reviewer does not have a direct relationship to a Movie, how can a Movie list the names of it's Reviewers? What would you call this relationship?

Review would have it's own table with columns for both user and movie - it would act as a join table. So a user could have many movies through reviews and reviews could have many users through reviews.


<p class='util--hide'>View <a href='https://learn.co/lessons/week-2-day-4-discussion'>Domain Modelling</a> on Learn.co and start learning to code for free.</p>
