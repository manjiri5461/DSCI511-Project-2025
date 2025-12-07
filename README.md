# DSCI511-Project-2025
Our project processes US National Park Services data sourced from various API endpoints and raw data chunks. The goal was to extract, clean, merge and prepare the data for further data analytics and visualization.The objective of this project is to provide potential national park guests with the ability to find a location that best aligns with their goals for their trip; seeing as a large number of travelers utilized the existing unoptimized sites, amelioration of this process is much needed. All data being accessed for this process is public domain as it comes directly from the United States government, but credit must be given if the data is republished in any manner. While we have free access to the data, it is limited to amenities and activities set on park land, not the surrounding areas. Our group members have both the coding experience and design competency to create the dataset and communicate our findings, so we are confident in our ability to undertake a project of this nature.

## Group Members: Anna Grace, Manjiri Khodke, Andrea MacGregor, Morgan Murphy

## Steps Performed: 

1. Data Acquisition
Parsed .txt API dumps containing nested JSON.
Extracted relevant fields manually since API pagination limits prevented automated bulk downloads.

3. Data Cleaning
-Standardized column names
-Removed HTML tags using BeautifulSoup
-Fixed mojibake text issues (â€”)
-Normalized whitespace
-Parsed activities from strings to Python lists
-Split activity info into activity_names and activity_ids
-Removed duplicates
-Converted descriptions to clean UTF-8
-Preserved missing latitude/longitude as NaN
-Saved final cleaned CSV

## Chalenges Faced

1. Fixed broken encodings(mojibake)
2. Parsing issues with the activities columns because initialilly it was saved as string while we wanted them as lists but we solved that issue. 
3. Few json files were nested deeply, had some missing keys and had inconsistent structures - fixed.
4. Merging Limitations - Because data had a few missing  park codes, we could not categorize every park. This becomes a known limitation.

