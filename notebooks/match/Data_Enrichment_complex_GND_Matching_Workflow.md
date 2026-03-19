Step 1: Data Enrichment (LibraryTool)
First, use the LibraryTool (Excel Alma Lookup Tool) to enrich your initial dataset with administrative and bibliographic metadata from Alma.

Guide: https://pul-confluence.atlassian.net/wiki/spaces/ALMA/pages/1770449/Excel+Alma+Lookup+Tool

Goal: Ensure your starting Excel file has the necessary identifiers and base metadata.

Step 2: Clean up and Format (Python)
Once you have your enriched Excel file, use Python scripts in this to prepare the data for matching.

Specific Action: Separate the variants so they can be processed correctly. * Details: This step involves splitting multi-value cells (e.g., names separated by pipes | or commas ,) into individual rows or cleaned lists. This ensures that the matching service in the next step can evaluate each name variant individually.

Step 3: Fine-tuning & GND Matching (OpenRefine)
The final matching is performed using OpenRefine to handle fuzzy logic and direct reconciliation with the Lobid/GND database.

Tutorial: https://blog.lobid.org/2018/08/27/openrefine.html

Goal: Use the Lobid reconciliation service to link your local entities to official GND URIs.
