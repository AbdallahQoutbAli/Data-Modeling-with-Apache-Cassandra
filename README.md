# Data-Engineer-Nanodegree-Projects-Udacity
Projects done in the [Data Engineer Nanodegree by Udacity.com](https://www.udacity.com/course/data-engineer-nanodegree--nd027)

#### Project 1: Data Modeling with Postgres and Apache Cassandra


#### The image below is a screenshot of what the denormalized data should appear like in the event_datafile_new.csv 

![image](https://user-images.githubusercontent.com/47276503/218794760-3c216787-ee1d-4277-97a0-bb713591ad43.png)

<p> 
The Business Asked to made the Below Query Give me the artist, song title and song's length in the music app history <br> that was heard during sessionId = 338, and itemInSession = 
<br>
<h2> First Create Table Table song_info And Choose only the Columns Asked To load  </h2>
<br>

``` sql 
query =
    
    Create table if not exists song_info (
    artist text , 
    song_title text,
    length float ,
    session_id int,  
    item_session int, 
    Primary key (session_id,item_session)
    )

 
```
Note :
For the Above Query , the session_id and Column item_session was used as a partition key because the queries will filter by them 
and used as clustering columns to help make up a unique key.
<p> 


 <h2> The Below Query Load Data Inside Table Song_info  </h2>

![image](https://user-images.githubusercontent.com/47276503/218798640-3c3de9c2-7cd2-4390-8cf4-676fdb1160b2.png)



 <h2> SELECT to verify that the data have been inserted into each table </h2>

![image](https://user-images.githubusercontent.com/47276503/218798817-a8c3f13a-5ffb-4934-9d36-d0186748ba5a.png)



Thanks !

Email : Abdallah.Qoutb@gmail.com
Data Engineer
