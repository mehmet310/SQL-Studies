# SQL Study-6
## Questions:
- Perform the following query scenarios on the dvdrental sample database.
1) What is the average of the values in the rental_rate column in the movie table?
2) How many of the movies in the movie table start with the character 'C'?
3) Among the movies in the movie table, how many minutes is the longest (length) movie with a rental_rate equal to 0.99?
4) How many different replacement_cost values ​​are there for the movies longer than 150 minutes in the movie table?

## Answers:
1) **SELECT AVG**(rental_rate) **FROM** film
2) **SELECT COUNT**(rental_rate) **FROM** film **WHERE** title **LIKE** 'C%';
3) **SELECT MAX**(length) **FROM** film **WHERE** rental_rate = 0.99;
4) **SELECT COUNT**(DISTINCT replacement_cost) **FROM** film **WHERE** length>150;
