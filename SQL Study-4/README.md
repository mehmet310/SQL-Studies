# SQL Study-4

## Questions:
- Perform the following query scenarios on the dvdrental sample database.
1) Sort the different values in the replacement_cost column in the movie table.
2) How many different data are there in the replacement_cost column in the movie table?
3) How many of the movie titles in the movie table start with the character T and at the same time the rating is equal to 'G'?
4) How many of the country names (country) in the country table consist of 5 characters?
5) How many of the city names in the city table end with the character 'R' or r?

## Answers:

1) **SELECT DISTINCT** replacement_cost **FROM** film;
2) **SELECT COUNT** (**DISTINCT** replacement_cost) **FROM** film;
3) **SELECT COUNT** (title) **FROM** film **WHERE** title **LIKE** 'T%' **AND** rating='G';
4) **SELECT COUNT** (country) **FROM** country **WHERE** country **LIKE** '_____';
5) **SELECT COUNT**(city) **FROM** city **WHERE** city **ILIKE** '%r';
 
