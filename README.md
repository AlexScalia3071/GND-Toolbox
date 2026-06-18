# GND-Toolbox

A small Python project to support work with data from the **GND (Gemeinsame Normdatei)** and related authority files.

This project helps:
- Clean and standardize metadata
- Match or correct entries (e.g. names, institutions)
- Use AI to assist with data tasks
- Pull authority information (e.g. from LoC, GND, Wikidata)

Folder Breakdown:
find/: Contains code regarding finding and isolating information within the GND database or local lists. This includes streaming through massive MARCXML dumps to pull out specific project IDs or searching for particular academic keywords to segment the data.

match/: Contains scripts regarding finding matching records across your datasets. This code handles your lookup maps and "Waterfall" priority matching strategies to find where your local records explicitly align with GND properties.
