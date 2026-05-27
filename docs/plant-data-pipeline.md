# Plant Data Pipeline

ecokeeper uses external plant data as a starting point for search, filtering, and garden-planning features.

The plant data pipeline ingests, normalizes, and enriches records so the app can present more useful plant information to users while supporting performant search and filtering.

## Goals

- Ingest plant records from external sources
- Normalize inconsistent fields across records
- Enrich records for search, filtering, and display
- Support scientific names, common names, distributions, images, and related metadata where available
- Prepare data for backend APIs used by the mobile app

## Challenges

External plant data can be inconsistent across endpoints and records. Some records may have richer metadata than others, and related species or subspecies may expose different levels of detail.

The pipeline needs to preserve useful plant information while avoiding duplicate or confusing records in the user experience.

## Pipeline overview

1. Fetch plant records from external sources
2. Normalize key fields such as scientific name, common names, images, distributions, and metadata
3. Resolve duplicate or related records where appropriate
4. Store normalized records in the application database
5. Index plant data for search and filtering
6. Expose plant records through backend API endpoints used by the mobile app

## Product impact

This pipeline supports the app’s plant search and planning experience by making plant records easier to search, filter, and present in a user-friendly way.

Better data quality helps users narrow plant options based on garden conditions and reduces friction when choosing plants for a specific site.

## Technical areas demonstrated

- ETL workflow design
- Data normalization
- Backend API support
- Search indexing
- Product-aware data modeling
- Handling imperfect third-party data
