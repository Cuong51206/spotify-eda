# Spotify Tracks Exploratory Data Analysis (EDA)

## Project Overview
This project performs an in-depth Exploratory Data Analysis (EDA) on Spotify datasets to uncover historical musical trends and understand the underlying relationships between various audio features (such as acousticness, energy, and loudness) and overall track popularity. 

## Source
* **Source:** [Spotify Dataset on Kaggle](https://www.kaggle.com/datasets/lehaknarnauli/spotify-datasets)

## Key Findings

Based on the exploratory data analysis and data visualization, four major trends were identified:

1. **Strong Positive Correlation Between Energy and Loudness:**
   * *Evidence:* Pearson correlation matrix and `Loudness vs Energy` regression plot.
   * *Analysis:* The data confirms a direct physical relationship in modern music production: highly energetic tracks are mixed to be noticeably louder. This aligns perfectly with the recording industry's "Loudness War," where producers maximize loudness to drive emotional impact and capture listener attention.

2. **Acousticness is Inversely Proportional to Popularity:**
   * *Evidence:* `Popularity vs Acousticness` regression plot.
   * *Analysis:* Purely acoustic tracks (featuring live instruments with minimal electronic processing) score significantly lower in popularity metrics. This heavily reflects current Spotify user demographics and preferences, which lean toward electronic-driven genres like Pop, Hip-hop, and EDM over traditional Folk or Classical music.

3. **Song Duration Fluctuates by Decade with Recent Standardization:**
   * *Evidence:* `Year vs Duration` line plot and bar chart.
   * *Analysis:* Track durations exhibited massive variance from the 1920s through the 1980s. However, lengths began to stabilize in the 2000s and have shown a distinct **downward trend** from 2010 to 2020. This is a clear indicator of the Streaming Era's impact, where artists actively optimize track lengths to suit recommendation algorithms and maximize stream counts.

4. **Genre Context Dictates Both Duration and Popularity:**
   * *Evidence:* Genre-based bar charts derived from `SpotifyFeatures.csv`.
   * *Analysis:* The data refutes the straightforward assumption that longer tracks equate to higher popularity. Genres with the highest average durations are *Children's Music* and *Classical*, whereas the most popular genres are *Comedy* and *Pop*. Therefore, the genre context—rather than raw duration—is the primary driver of listener engagement.
