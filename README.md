# ecokeeper case study

ecokeeper is a native habitat and garden-planning app that helps people understand their garden conditions and make more thoughtful planting decisions.

This repository documents selected technical and product work from the project. The production codebase is private, but this case study summarizes architecture, product decisions, data workflows, and release processes.

## Product scope

ecokeeper supports:

- Garden setup and location-based planning
- Garden sections and section-level observations
- Sunlight tracking over time
- Plant search and filtering
- Journal entries and notes
- Subscription-gated access
- Beta testing and product iteration

## Technical scope

The project includes:

- React Native / Expo mobile application
- TypeScript frontend architecture
- Backend API services
- Authentication workflows
- Subscription and app-store billing integration
- ETL workflows for external plant data
- Search optimization and indexing
- OTA update strategy
- iOS and Android release workflows

## Selected writeups

- [Architecture overview](docs/architecture.md)
- [Plant data pipeline](docs/plant-data-pipeline.md)
- [Search performance](docs/search-performance.md)
- [Release workflow](docs/release-workflow.md)
