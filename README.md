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
