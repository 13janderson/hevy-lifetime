## How to use

1. Export data from hevy app as csv: settings -> Export & Import data. This is our lifetime data, despite the free version of hevy only **showing** your workout progress over the past 3 months.
2. Run `python append_new_records.py <MASTER_PATH> <NEW_DATA_PATH>`
- <MASTER_PATH> is where we store the accumulated data over time, so you run this program intermittently to update the global data and have graphs of the global data.
    - Initially, we have no data to add to so use the provided **blank_master_data.xlsx** to populate an empty master data file..
- <NEW_DATA_PATH> is the pointer to our latest data that we want to insert, this is simply the **workout.csv** file exported from hevy.
- TLDR:
    - Initial use: `cp blank_master_data.xlsx master_data.xlsx`; `python blank_master_data.xlsx workout_data.csv`
    - Incremental use: `python master_data.xlsx workout_data.csv`.

