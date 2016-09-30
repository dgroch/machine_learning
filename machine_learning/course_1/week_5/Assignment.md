# Assignment :: Week 5

1. Counting unique users: The method .unique() can be used to select the unique elements in a column of data. In this question, you will compute the number of unique users who have listened to songs by various artists. For example, to find out the number of unique users who listened to songs by 'Kanye West', all you need to do is select the rows of the song data where the artist is 'Kanye West', and then count the number of unique entries in the ‘user_id’ column.

** Question 1: Compute the number of unique listeners for each of these artists: **

1. 'Kanye West' => 3775
2. 'Foo Fighters' => 3429
3. 'Taylor Swift' => 6227
4. 'Lady GaGa' => 4129

** Question 2 **

Use the `.groupby` method to aggregate listen count for each song and then sort the resulting SFrame according to the ‘total_count’, and find the artist with the most popular and least popular artist in the dataset. Save these results to answer the quiz at the end.

* Least popular => William Tabbert	(14)
* Most Popular => Kings of Leon (43218)

** Question 3 **

Using groupby-aggregate to find the most recommended songs: Now that we learned how to use .groupby() to compute aggregates for each value in a column, let’s use to find the song that is most recommended by the personalized_model model we learned in the iPython notebook above.

* Least recommended => {'count': 1, 'song': "The Lighthouse's Tale - Nickel Creek"}
* Most recommended => {'count': 453, 'song': 'Undo - Björk'}
