# 100 days of code challenge (SQL)

#### Day 1: November 15, 2022

##### **Today's Progress:** Today I began querying a London Bus Injury dataset where I set out to answer multiple questions that I came up with based on the data. 

##### **Thoughts:** It was really satisfying troubleshooting my failed queries, I relied on the StackOverflow community to help me figure out why I wasn't getting a decimal value for a percentage I was trying to calculate (was told to use 100.00 instead of 100). I'm proud that I was successful in my work and am excited to continue gathering insights tomorrow. 

##### **Skills Used:** 

    1. WHERE statements
    2. GROUP BY statements
    3. ORDER BY statements
    4. COUNT()
    5. DESC
    6. CAST() AS DECIMAL (10,2)
    7. VIEWS
    8. INNER JOIN statements
    9. VIEWS based on INNER JOINS
    10. LIKE '%'

##### **Link to work:** [Click here to see my code](https://github.com/ashlyn-musgrave/100-Days-of-Code-Challenge-SQL/blob/main/Day%201%20-%20Bus%20Safety.sql)

#### Day 2: November 16, 2022

##### **Today's Progress:** Today I worked with the same London Bus Safety dataset and looked at the most dangerous/safest Boroughs in terms of Bus accidents. I also looked at the total number of victims per incident type. 

##### **Thoughts:** I felt a lot more confident querying this dataset today, I had a really long process in my head for how to do something and figured out a way to shorten it and create less work. I'm skill getting an error when trying to PIVOT my table but will keep trying until I get it. 

##### **Skills Used:**  

    1. OUTER JOIN
    2. UNION
    3. PIVOT

##### **Link to work:** [Click here to see my code](https://github.com/ashlyn-musgrave/100-Days-of-Code-Challenge-SQL/blob/main/Day%202%20-%20Bus%20Safety.sql)

#### Day 3: November 17, 2022

##### **Today's Progress:** Today I continued working on the London Bus Safety dataset to work through my PIVOT error. With a LOT of help from online resources, I successfully pivoted the table! There is however a column that's not appearing in the dataset that's supposed to be there so that's what I'll be troubleshooting tomorrow.

##### **Thoughts:** I'm thrilled that I made progress today on the PIVOT query. I'm not sure why the Incident Type isn't showing up in the table, I'm thinking it has something to do with needed to add an order by statement. Stay tuned...

##### **Skills Used:** 

    1. PIVOT

##### **Link to work:** [Click here to see my code](https://github.com/ashlyn-musgrave/100-Days-of-Code-Challenge-SQL/blob/main/Day%203%20-%20Bus%20Safety.sql)


#### Day 4: November 19, 2022

##### **Today's Progress:** Today I finally got my desired result working with my PIVOT table! I tried to replace all the NULL values with 0 but wanted to move on since I wasn't making much progress. I'm planning to tackle that once I start data cleaning. I went back to one of my previous queries and tried to clean it up by deleting duplicate columns after a join. Still haven't worked that out yet but will keep trying.

##### **Thoughts:** So excited that my PIVOT table turned out correctly, I feel so much accomplishment from that. Updating all the NULL values with a zero is proving difficult for me since I performed my PIVOT based on a VIEW. When I start the data cleaning portion of this project, I'll tackle that subject. I'm also trying to figure out where I'm going wrong with getting duplicate tables after a join. Seeking help if anyone is out there...

##### **Skills Used:** 
    1. PIVOT
    2. UPDATE
    3. FULL OUTER JOIN 
    4. RIGHT OUTER JOIN
 
##### **Link to work:** [Click here to see my code](https://github.com/ashlyn-musgrave/100-Days-of-Code-Challenge-SQL/blob/main/Day%204%20-%20Bus%20Safety.sql)

#### Day 5: November 20, 2022

##### **Today's Progress:** Today I continued working on the Bus Safety dataset and worked on cleaning up my past query results, specifically the duplicate columns in the injury severity table and updating the NULL values to zeros. I also found the top 5 routes with the most accidents. 

##### **Thoughts:** I couldn't find an option to join my injury severity tables together where the duplicate coloumn was deleted (but still wanting to keep the initial column) so instead I exported the joined tables to Excel, deleted the duplicates there, then imported it back into SMSS. From there, I started updating all the NULL values to zeros and was 75% successful. For some reason, it's not updating the percent_fatal coloumn when I run my query but it is for everything else. Will work out a solution for this next time... 

##### **Skills Used:** 
    1. UPDATE
    2. ISNULL( , )
    3. Exporting/Importing data from Excel
 
##### **Link to work:** [Click here to see my code](https://github.com/ashlyn-musgrave/100-Days-of-Code-Challenge-SQL/blob/main/Day%205%20-%20Bus%20Safety.sql)


#### Day 6: November 21, 2022

##### **Today's Progress:** Today I worked through my error when trying to update NULL values to zero for one of my columns in the Injury_Severity table. After a LOT of research and trial and error, I was successful! 

##### **Thoughts:** The root of the problem was that the data type for the percent_fatal coloum was NVARCHAR(255) when it should've been (float, null). I'm still not sure how this coloumn's data type was different from all the rest but nevertheless I replaced the non numeric values to NULL and then altered the data type. I finally have the info I need to start on data visualization in Tableau!

##### **Skills Used:** 
    1. ALTER TABLE
    2. SET
    3. CASE
    4. ISNUMERIC
    5. Table Renaming 
 
##### **Link to work:** [Click here to see my code](https://github.com/ashlyn-musgrave/100-Days-of-Code-Challenge-SQL/blob/main/Day%206%20-%20Bus%20Safety.sql)
