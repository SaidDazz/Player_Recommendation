# Football Player Recommendation Engine

## Overview
The **Player Scouting Recommendation System** helps users identify football players with similar playing styles based on key statistical metrics. By entering a player's name, the system returns a list of the top 10 most similar players, utilizing cosine similarity for precise matches. Powered by **Apache Solr** for data storage and **Streamlit** for a user-friendly interface, this tool is designed for analysts, scouts, and football enthusiasts.

## Table of Contents
- [Project Structure](#project-structure)
- [Key Features](#key-features)
- [Requirements](#requirements)
- [Setup and Installation](#setup-and-installation)
- [Interface Overview](#interface-overview)
- [Contributors](#contributors)

## Project Structure

- **`img/`**: Contains image assets for the interface.
- **`app.py`**: The main Streamlit application file.
- **`docker-compose.yml`**: Docker configuration file for running Apache Solr.
- **`players.csv`**: Dataset with player statistics.
- **`README.md`**: Documentation for the project.
- **`requirements.txt`**: Lists the Python libraries required.
- **`solr.ipynb`**: Jupyter Notebook for interacting with Solr and running queries.

## Key Features
- **Player Search**: Find a player by name and view detailed statistics such as goals, assists, expected goals (xG), expected assists (xA), and other key metrics.
- **Player Recommendations**: Get a list of the top 10 players with similar statistics based on cosine similarity.
- **Visual Comparisons**: Compare players visually with radar charts to easily analyze their strengths and weaknesses.

## Requirements
- **Docker**: To set up and run Apache Solr.
- **Python 3.7+**: With the following packages installed:
  - `streamlit`
  - `requests`
  - `pandas`
  - `scikit-learn`

## Setup and Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/SaidDazz/player_recommendation.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd player_recommendation
    ```

3. **Set up Apache Solr with Docker**:
    ```bash
    docker-compose up -d
    ```

4. **Install Python dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

5. **Run the Streamlit app**:
    ```bash
    streamlit run app.py
    ```

## Interface Overview
The **Player Scouting Recommendation System** interface allows users to search for a player, view detailed statistics, and see the top recommendations based on similarity:

![Player Scouting Recommendation System Interface](./img/ziyech.jpg)

In the example above, a search for **Hakim Ziyech** shows his key stats and the top 10 similar players.

## Contributors

- **Ahmed Said Dazzazi** – Data Engineering Specialist

---
