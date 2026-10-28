# Choreography Creation: Music vs Silence

## Assignment Brief

This project is part of the Data Centric Programming module. It involves collecting an original dataset through personal observation, storing and validating the data, analysing it with Python, and developing an interactive application to explore the results.

The dataset for this project will be collected manually. No downloaded, scraped, AI-generated, or retrospectively estimated data will be used.

## Questions

The project aims to investigate my personal choreography creation process and explore the possible relationship between music and creative activity.

The main research questions are:

1. Do I spend more time creating choreography when listening to music or when working in silence?
2. Does the number of new dance movements or sequences differ between sessions with music and sessions without music?
3. Is my self-rated creativity associated with the duration of a choreography session?

These questions will guide the data collection and analysis. The conclusions will be based on the observations collected throughout the semester.

## Data Dictionary

Each row in the dataset will represent one choreography creation session. If I have multiple sessions on the same day, each session will be recorded separately.

| Column | Data type | Description | Measurement method |
|---|---|---|---|
| `date` | DATE | Date of the session | Recorded on the day of the session |
| `duration_minutes` | INTEGER | Duration of the session in minutes | Measured using a stopwatch |
| `music` | TEXT | Whether music was used (`yes` or `no`) | Recorded after the session |
| `music_genre` | TEXT | Genre of music used, or `none` | Recorded based on the music played |
| `location` | TEXT | Location where the session took place | Recorded after the session |
| `ideas_created` | INTEGER | Number of new movements or sequences created | Counted using a consistent counting rule |
| `creativity_rating` | INTEGER | Subjective creativity rating from 1 to 5 | Self-assessed immediately after the session |

### Data Collection Rules
I will record each session on the day it takes place.
I will measure session duration using my phone.
I will use the same definition of a new movement or sequence throughout the project.
When music is not used, `music_genre` will be recorded as `none`.
Missing observations will not be invented or reconstructed later.
Data types, missing values and invalid values will be checked when the data is loaded into the database.

## Description of the Project

The aim of this project is to investigate how the presence or absence of music relates to the time I spend creating choreography.

Choreography creation can involve experimenting with movements, connecting sequences, repeating ideas and developing new combinations. Music may influence this process, but the effect may differ between sessions.
I will collect original data from my own choreography sessions. I will record the duration of each session, whether music was used, the music genre where applicable, the location and the number of new ideas created.
The dataset will initially be stored in a CSV file in the repository.
The project will focus on my personal experience rather than attempting to generalise the findings to all dancers.

## Instructions for Use

### Current Status

This repository is currently at the proposal and data collection stage. 

### Planned Setup

Python 3 is required. 

## How It Works

The planned application will consist of the following stages.

1. **Data collection:** Record each choreography session manually in `choreography_data.csv`.
2. **Data validation:** Check dates, numeric values, categorical values and missing observations.
3. **Database storage:** Import the CSV records into an SQLite table.
etc

## Findings
