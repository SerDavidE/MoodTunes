# Moosic Playlist Automation with Data Science

**Moosic**, a startup specializing in curated playlists, aims to automate its playlist creation process using Data Science. This project leverages Spotify's audio features to cluster songs, potentially forming the basis for automated playlists.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Source and Description](#data-source-and-description)
3. [Methodology](#methodology)
4. [Results](#results)
5. [Discussion and Insights](#discussion-and-insights)
6. [Future Work](#future-work)
7. [How to Run the Code](#how-to-run-the-code)
8. [License](#license)

## Introduction
Moosic's unique value proposition is its expert-curated playlists that capture specific moods or styles. However, as the business scales, there's a need to speed up the playlist creation process. This project explores the potential of automating playlist curation using Spotify's audio features and K-Means clustering.

## Data Source and Description
The data has been sourced from the Spotify API, which provides various audio features for songs. Features include:
- 'danceability'
- 'energy'
- 'key'
- 'loudness'
- 'mode'
- 'speechiness'
- 'acousticness'
- 'instrumentalness'
- 'liveness'
- 'valence'
- 'tempo'

## Methodology
1. **Data Cleaning**: Removed unnecessary columns and handled missing values.
2. **Feature Scaling**: Used Standard Scaling to normalize the feature set.
3. **Clustering**: Applied K-Means clustering to group songs based on their audio features.

## Balancing Tech with Business
Technical Methods suggested optimal clusters around 4 or 5, but the ideal number of clusters can be subjective.
Business Requirements:

- Playlists should contain between 50 and 250 songs.
- Given a dataset of 5,000 songs, this implies 20 to 100 clusters.
- Implication: Business constraints may push for more clusters to ensure playlist sizes are manageable.

## Results
The songs were clustered into groups, potentially forming the basis for playlists. Initial clusters (for k=4 and k=5) were labeled based on the dominant audio features.

## Discussion and Insights
The clusters provide insights into the nature of songs and their potential mood or style. This serves as a starting point for automating the playlist creation process. However, collaboration with music experts is essential to refine and validate these playlists.

## Future Work
- Explore other clustering algorithms.
- Incorporate feedback from music experts for playlist refinement.
- Consider other features like song lyrics for a more comprehensive clustering.

## How to Run the Code
1. Clone the repository.
2. Ensure you have the required libraries installed. You can install them using the command `pip install -r requirements.txt` (Note: This assumes you have a `requirements.txt` file).
3. Run the Jupyter notebook or Python script.

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details (Note: You'd need to include a license file if you mention this).
