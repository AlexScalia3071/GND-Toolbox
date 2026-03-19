Step 1: Data Enrichment (LibraryTool)
Before running any Python scripts, use the LibraryTool (Excel Alma Lookup Tool) to enrich your initial dataset with administrative and bibliographic metadata from Alma.

Guide: Excel Alma Lookup Tool Instructions

Goal: Ensure your starting Excel file has the necessary identifiers and base metadata.

Step 2: Data Cleaning (Python)
Once you have your enriched Excel file, use the scripts in this repository to clean and segment the data.

Goal: Standardize names, remove "noise" (accents/special characters), and prepare the file for reconciliation.

Step 3: Fine-tuning & GND Matching (OpenRefine)
The final matching is performed using OpenRefine to handle fuzzy logic and direct reconciliation with the Lobid/GND database.

Tutorial: Reconciling with the GND in OpenRefine

Goal: Use the Lobid reconciliation service to link your local entities to official GND URIs.
