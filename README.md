# Movie Ratings Data Analysis Project

## Project Overview

This project involves hypothesis testing on movie ratings data to explore various aspects of movie popularity, release year, viewer demographics, and social viewing preferences. Using a dataset of 400 movies rated by 1,097 participants, we investigate factors influencing movie ratings, differences in rating patterns among demographic groups, and the effects of social watching behavior on viewer enjoyment.

## Dataset

The dataset used in this analysis includes ratings for 400 movies along with additional demographic and behavioral data from each participant. Key columns in the dataset include:

- **Movie Ratings (Columns 1-400)**: Ratings on a scale of 0-4 for each movie.
- **Sensation Seeking (Columns 401-421)**: Self-assessed scores on sensation-seeking behaviors (1-5 scale).
- **Personality Questions (Columns 422-464)**: Responses to various personality questions (1-5 scale).
- **Movie Experience Ratings (Columns 465-474)**: Self-reported movie experience ratings (1-5 scale).
- **Demographic Attributes**:
  - **Gender Identity** (Column 475): Coded as 1 for female, 2 for male, 3 for self-described.
  - **Only Child** (Column 476): Coded as 1 for only child, 0 for siblings, -1 for no response.
  - **Social Viewing Preference** (Column 477): Coded as 1 for preferring to watch alone, 0 for socially, -1 for no response.

## Analysis Overview

1. **Popularity and Ratings**: 
   - Hypothesis: Popular movies (more ratings) are rated higher than less popular movies.
   - Method: Median split of ratings count and a Mann-Whitney U test.
   
2. **Years of Release and Ratings**:
   - Hypothesis: Newer movies are rated differently than older ones.
   - Method: Median split of release years and Mann-Whitney U and KS tests.

3. **Gender and Movie Enjoyment**:
   - Analysis includes tests for gender-based enjoyment differences in specific movies like "Shrek (2001)" and examines the proportion of movies rated differently by male and female viewers.

4. **Only Child Effect**:
   - Hypothesis: Differences in movie enjoyment between only children and participants with siblings.
   - Specific analysis of movies like "The Lion King (1994)" and general tests across all movies.

5. **Social Watching Effect**:
   - Examines whether social viewing preferences affect enjoyment, using "The Wolf of Wall Street (2013)" as a case study and general tests across all movies.

6. **Ratings Distribution**:
   - Comparison of ratings distribution for specific movies, such as "Home Alone (1990)" versus "Finding Nemo (2003)."

7. **Quality Consistency Across Franchises**:
   - Tests for consistency of movie quality in franchises like "Star Wars," "Harry Potter," and "Jurassic Park" using the Kruskal-Wallis test.

8. **Additional Finding**:
   - Observed higher average movie-watching interest among male participants, confirmed by a Welch t-test for significance.

## Key Findings

- **Popularity Impact**: Higher popularity correlates with higher ratings.
- **Newer Movies**: Significant rating differences between newer and older movies.
- **Gender Differences**: Small proportion of movies showed significant rating differences between genders.
- **Sibling Influence**: Minimal effect of being an only child on movie enjoyment.
- **Social Viewing**: Limited evidence supporting the social watching effect across most movies.
- **Franchise Quality**: Inconsistent quality was found in several franchises, including "Star Wars" and "Toy Story."
