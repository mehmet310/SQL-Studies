# SQL Study-3
## Questions
- Perform the following query scenarios on the dvd rental sample database.

1) List the country names in the country column of the country table, starting with the 'A' character and ending with the 'a' character.

2) List the country names in the country column of the country table, consisting of at least 6 characters and ending with the 'n' character.

3) In the title column of the movie table, list the movie names containing at least 4 'T' characters, regardless of upper or lower case letters.

4) From the data in all the columns in the movie table, sort the data that starts with the title 'C' character, has a length greater than 90 and a rental_rate of 2.99.

## Answers

1) **SELECT** * **FROM** country **WHERE** country **LIKE** 'A%a';

2) **SELECT** * **FROM** country **WHERE** country **LIKE** '_____%n';

3) **SELECT** title **FROM** film **WHERE** title **ILIKE** '%t%t%t%t%' ; 

4) **SELECT** * **FROM** film **WHERE** title **ILIKE** 'C%' **AND** rental_rate=2.99 **AND** length>90 ;
