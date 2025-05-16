# Supervised Learning Project: Ultra Trail Running Performance Optimization

## Project Overview
This project analyzes ultra trail running performance data to optimize athlete strategies during competitions. The focus is on activities lasting over 3 hours, analyzing various metrics including heart rate, altitude, speed, and other physiological and environmental factors.

## Data Processing
The project processes training data from JSON format files containing:
- Heart rate measurements
- Altitude data
- Distance covered
- Temperature readings
- Cadence information 
- Speed metrics

### Data Structure
- `full-data/`: Raw training session data in JSON format
- `long-tr-data/`: Processed CSV files containing filtered ultra trail running sessions (>3 hours)

### Processing Steps
1. Filter sessions by:
   - Sport type: TRAIL_RUNNING
   - Duration: > 3 hours
2. Extract and process metrics:
   - Convert timestamps to datetime
   - Calculate cumulative duration
   - Process distance and elevation differences
   - Merge all metrics into single dataframe

## Analysis
The project includes exploratory data analysis (EDA) examining:
- Time series analysis of key metrics
- Statistical distributions
- Correlation between different variables
- Rolling statistics for performance patterns

