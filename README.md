# GND-Toolbox

A Python project to streamline data management, entity matching, and direct authority file interactions for the GND (Gemeinsame Normdatei) and related metadata standards.

Key Features
Metadata Cleaning & Standardizing: Utilities to clean, parse, and normalize record sets.

Entity Matching: Automated mapping across datasets using structured lookup rules and waterfall matching logic.

GND API Operations (SRU Direct Interaction):

Query & Fetch: Retrieve authority information across multiple sources (GND, LoC, Wikidata).

CREATE Request: Generate and submit new GND records directly via the SRU interface.

REPLACE Request: Submit updated record payloads to modify existing GND entries via SRU.

AI-Assisted Processing: AI workflows integrated into key metadata processing tasks.

Folder Structure
api/ 

Handles direct interaction with the GND SRU endpoint. Manages connection parameters, XML payload formatting, and execute CREATE and REPLACE write requests to create or update GND records.

find/

Code for locating and isolating target information within local files or the GND database. Handles streaming through large MARCXML dumps, isolating specific project IDs, and filtering data by academic keywords.

mapping/

Contains schema transformations, crosswalks, and field-mapping definitions used to align local data models with standard GND/MARC21 structures before processing or uploading.

match/

Scripts for cross-dataset record matching. Manages lookup tables and multi-tiered "waterfall" priority strategies to match local records against GND entities.
