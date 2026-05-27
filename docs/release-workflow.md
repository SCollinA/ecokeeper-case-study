# Release Workflow

ecokeeper is distributed as a mobile app through iOS and Android release channels. The release workflow includes native builds, app-store submission, beta testing, over-the-air updates, and environment-specific configuration.

This document summarizes the release process at a high level. The production codebase and private configuration are not included in this case study.

## Goals

The release workflow is designed to support:

- iOS and Android distribution
- Beta testing before wider release
- App Store and Play Store submission
- Over-the-air updates where appropriate
- Environment-specific configuration
- Stable release practices for a mobile product

## Release channels

The project supports separate release concerns for development, preview, beta, and production contexts.

These contexts may differ by:

- Build configuration
- API environment
- Authentication configuration
- Subscription/billing configuration
- App identifiers
- Distribution channel
- Testing audience

Separating these concerns helps reduce risk when testing app-store behavior, billing flows, and production-facing features.

## Native builds

Native builds are used when changes require app-store review or native configuration updates.

Examples include:

- Initial app submission
- Native dependency changes
- Bundle identifier or package configuration
- App Store / Play Store metadata requirements
- Subscription or billing-related review needs
- Platform-specific capabilities

## Over-the-air updates

Over-the-air updates are used for changes that do not require a new native build.

Examples include:

- JavaScript and UI changes
- Copy updates
- Product flow refinements
- API-backed behavior changes
- Minor fixes that do not alter native configuration

OTA updates allow faster iteration while still respecting the boundary between native app changes and app-store-reviewed changes.

## App-store submission

The app-store release process includes:

- Preparing native builds
- Validating platform requirements
- Submitting app metadata
- Managing screenshots and review information
- Responding to review feedback
- Coordinating subscription-related review requirements
- Testing production-like behavior before approval

## Beta testing

Beta testing supports validation before broader release.

Beta workflows include:

- Distributing test builds
- Collecting feedback
- Testing app-store subscription behavior
- Verifying onboarding and core product flows
- Confirming API and environment configuration
- Iterating on product issues before production release

## User-facing updates

The project includes mechanisms for communicating meaningful changes to users, especially when updates are delivered without a full app-store release.

This helps users understand what changed and supports a more transparent product experience.

## Release risks managed

The release workflow helps manage risks such as:

- Environment mismatch
- Incorrect app identifiers
- Auth configuration issues
- Billing/subscription configuration problems
- App-store review blockers
- Platform-specific behavior differences
- Users receiving stale or incompatible app versions

## Technical areas demonstrated

- Mobile release management
- Expo / React Native release workflows
- OTA update strategy
- iOS and Android app-store submission
- Environment-specific configuration
- Beta testing coordination
- Production-readiness planning
