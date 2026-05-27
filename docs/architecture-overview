# Architecture Overview

ecokeeper is a mobile-first garden and native habitat planning app. The app helps users organize gardens, track site conditions, and use plant data to make more thoughtful planting decisions.

This document summarizes the project architecture at a high level. The production codebase is private, but this case study outlines the major technical areas and product responsibilities.

## Goals

The architecture supports:

- Mobile-first garden planning
- Garden and section organization
- Sunlight tracking over time
- Plant search and filtering
- Journal entries and notes
- Subscription-gated access
- Beta testing and product iteration
- App Store and Play Store release workflows

## Mobile app

The mobile app is built with React Native and Expo.

The app includes flows for:

- Garden setup
- Section management
- Sunlight readings
- Plant search
- Plant association with garden sections
- Journal entries
- Onboarding
- Subscription access

The mobile architecture emphasizes clear product flows, reusable UI patterns, and a structure that supports iteration as the product grows.

## Backend API

The backend API supports app data, plant search, user-specific records, subscription access, and product workflows.

Backend responsibilities include:

- Serving garden and section data
- Supporting plant search and filtering
- Managing user-specific app data
- Supporting authentication-related workflows
- Supporting subscription-gated access
- Providing data to the mobile app through API endpoints

## Data workflows

ecokeeper uses external plant data as a starting point for search, filtering, and garden-planning features.

Data workflows include:

- Ingesting external plant records
- Normalizing inconsistent fields
- Enriching records for display and search
- Preparing data for backend API usage
- Indexing records for search performance

## Authentication and access

The app includes authentication and subscription-related workflows to support user accounts and paid access.

These workflows include:

- User sign-in and account access
- Subscription-aware app behavior
- App-store subscription integration
- Gated access to paid features

## Release architecture

The project uses a mobile release workflow that includes native builds, app-store submission, beta testing, and over-the-air updates.

Release concerns include:

- iOS and Android build configuration
- App Store and Play Store review requirements
- Beta distribution
- OTA update strategy
- Environment-specific configuration
- Release notes and user-facing update messaging

## Product architecture

The project is structured around real user workflows rather than isolated technical features.

Core product concepts include:

- Gardens
- Garden sections
- Sunlight observations
- Plants
- Journal entries
- Subscription access

This structure allows the app to guide users from basic garden setup toward more detailed site understanding and plant planning.

## Technical areas demonstrated

- React Native / Expo mobile development
- TypeScript application structure
- Backend API design
- ETL and data normalization
- Search optimization
- Authentication workflows
- Subscription workflows
- Mobile release management
- Product-minded architecture
