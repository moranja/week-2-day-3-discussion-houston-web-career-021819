# SQL Discussion Questions

### Talk with your table mates and write a few sentences about each question.

1 . When you tweet a tweet, your tweet is available to THE WHOLE INTERNET FOREVER. Why doesn't your tweet disappear after you post it? How does it stay on Twitter and stay associated to ​_your_​ account?

Twitter has a database to store all tweets. Some relational table that associates your tweets to you.

2 . When you enter your debit card into an ATM, how is your account identified? How does the bank associate that card number to your account? How does your bank store your account information? Do you think your address and phone number are stored the same way as your account number and how much money you have?

If each account is a row in a database, one column must be PIN code, one must be account number, etc. All things stored should be relatively secure, though I'd hope my PIN and balance are more secure than my address.

3 . How does Tinder know you are who you say you are when you open your application, type your password, and begin to swipe insatiably? How does it know that you and your latest match swiped right on each other, and that is wasn't someone other _John/Jane Doe_?

Keeps track of your username and password. Everything in SQL has a primary id, if you can just keep track of that then you don't have to worry about that it's someone with a different name.

4 . How do you think Yelp can show you all Latin Restaurants, with a $$ price rating, in the Financial District, which have higher than a 3 star rating?

SELECT * FROM restaurants WHERE type = 'Latin' AND price = '$$' AND location = 'Financial District' AND rating > 3;

 5 . What do you think this is doing:
```sql
SELECT * FROM artists WHERE ArtistName='Kid Cudi'
```

Return the entire row from the table "artists" in which the column "ArtistName" is equal to "Kid Cudi".

<p class='util--hide'>View <a href='https://learn.co/lessons/week-2-day-3-discussion'>SQL</a> on Learn.co and start learning to code for free.</p>
