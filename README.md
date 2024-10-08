# Analytics Pipeline

## Overview

This project is focused on building an ETL pipeline to gather data from multiple sources, clean and process it, and then structure it for analysis.

## Project Structure

- **`cached_data.py`**: Handles caching of player data to optimize repeated data access.
- **`data_provider.py`**: Provides utilities for reading and writing data in various formats.
- **`fact_bet.py`**: Transforms transaction data into a fact table for bets.
- **`game_dimension.py`**: Processes game-related data into a dimensional table.
- **`player_dimension.py`**: Processes player data into a dimensional table.
- **`run.py`**: Orchestrates the execution of the entire pipeline.
- **`spark_utils.py`**: Contains utility functions for interacting with Apache Spark.
- **`test_player_game.py`**: Unit tests for validating the transformation logic in `player_dimension.py`.

## Usage

1. **Setup**: Ensure Apache Spark is installed and properly configured.
2. **Execution**: Run the pipeline using the command:
   ```bash
   python run.py
