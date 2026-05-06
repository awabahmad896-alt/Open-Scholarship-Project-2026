# Van Gogh Open Heritage Project

## Project Description
Research Purpose: Exploring Vincent van Gogh artworks and metadata 
across European cultural heritage institutions using the Europeana API.

## Data Origin
- Source: Europeana API (https://api.europeana.eu/)
- Date accessed: May 2026
- License: Varies per record (CC0, CC BY, CC BY-SA, InC)
- Description: Metadata records of cultural heritage objects 
  attributed to Vincent van Gogh retrieved from Europeana

## Data Files
- [vangogh_europeana_raw.csv](data/vangogh_europeana_raw.csv) — Raw dataset (1707 records)
- [vangogh_europeana_clean.csv](data/vangogh_europeana_clean.csv) — Cleaned dataset (229 records)

## What has been done to the data
1. Retrieved raw data via Europeana API (1707 records)
2. Filtered by creator name to remove non-Van Gogh records
3. Selected 12 most useful columns
4. Fixed character encoding issues
5. Saved clean version as separate file

## What is missing or uncertain
- Many records have no year field
- Creator name is recorded differently across institutions
- Some records are about Van Gogh (books, journals) not by him

## Initial Research Steps
1. Accessed Europeana Search API using apidemo key
2. Queried all records containing "Van Gogh"
3. Retrieved 1707 records across multiple pages
4. Filtered by dcCreator field to keep only Van Gogh records
5. Extracted 12 key columns and fixed encoding
6. Saved both raw and clean datasets as CSV files
