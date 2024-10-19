# Spotify_Data_Analysis_using_SQL
Dataset :-  [Click here to get dataset](https://www.kaggle.com/datasets/sanjanchaudhari/spotify-dataset)
![spotify_logo](https://github.com/user-attachments/assets/2c1ff0c4-aa09-4640-93a3-80f7f53b3920)

# Overview
This project focuses on leveraging SQL to analyze a comprehensive Spotify dataset, encompassing details about tracks, albums, and artists. It entails transforming a denormalized dataset into a normalized structure, executing SQL queries across different complexity levels, and enhancing query efficiency. The project’s core aim is to refine advanced SQL techniques and extract meaningful insights from the dataset.

```sql
DROP TABLE IF EXISTS soptify;

CREATE TABLE spotify (
    artist VARCHAR(255),
    track VARCHAR(255),
    album VARCHAR(255),
    album_type VARCHAR(50),
    danceability FLOAT,
    energy FLOAT,
    loudness FLOAT,
    speechiness FLOAT,
    acousticness FLOAT,
    instrumentalness FLOAT,
    liveness FLOAT,
    valence FLOAT,
    tempo FLOAT,
    duration_min FLOAT,
    title VARCHAR(255),
    channel VARCHAR(255),
    views FLOAT,
    likes BIGINT,
    comments BIGINT,
    licensed BOOLEAN,
    official_video BOOLEAN,
    stream BIGINT,
    energy_liveness FLOAT,
    most_played_on VARCHAR(50)
);
```


# Data Dictionary

Before diving into SQL, it’s vital to get a solid understanding of the dataset. This dataset includes:

* Artist: The performer of each track.
* Track: The song's title.
* Album: The collection that features the track.
* Album Type: Classification of the album (e.g., single or full album).
* Various Metrics: Attributes like danceability, energy, loudness, tempo, and more.


# Finding Insights

Easy Level
1. Retrieve the names of all tracks that have more than 1 billion streams.
2. List all albums along with their respective artists.
3. Get the total number of comments for tracks where licensed = TRUE.
4. Find all tracks that belong to the album type single.
5. Count the total number of tracks by each artist.

Medium Level

6. Calculate the average danceability of tracks in each album.
7. Find the top 5 tracks with the highest energy values.
8. List all tracks along with their views and likes where official_video = TRUE.
9. For each album, calculate the total views of all associated tracks.
10. Retrieve the track names that have been streamed on Spotify more than YouTube.

Advanced Level

11. Find the top 3 most-viewed tracks for each artist using window functions.
12. Write a query to find tracks where the liveness score is above the average.
13. Use a WITH clause to calculate the difference between the highest and lowest energy values for tracks in each album.
