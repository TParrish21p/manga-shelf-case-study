# Manga Shelf

Manga Shelf is a Flutter/Firebase Android app for tracking a physical manga collection.

I built it because I wanted a simple, practical way to keep up with what manga I own, what I’m missing, and how my collection is organized across shelves. The goal was to make something useful for real collectors without turning it into a cluttered database app.

> Published under Bizarre Studios. Built by Tyler Parrish.

## Live App

Google Play: Approved for publication // updating with link when live

## What the app does

Manga Shelf helps users:

- track physical manga series and volumes
- organize manga across multiple custom shelves
- track owned, published, and missing volumes
- add reading status, genre, publisher, and notes
- upload custom cover images
- search metadata to prefill manga details
- view collection stats from a home dashboard
- use email/password login or Google Sign-In
- delete app data or delete their account from settings

## Screenshots

| Home | Collection | Add Manga |
|---|---|---|
| ![Home screen](screenshots/home.png) | ![Collection screen](screenshots/collection.png) | ![Add manga screen](screenshots/add-manga.png) |

| Shelves | Manga Detail | Settings |
|---|---|---|
| ![Shelves screen](screenshots/shelves.png) | ![Manga detail screen](screenshots/manga-detail.png) | ![Settings screen](screenshots/settings.png) |

## Tech stack

- Flutter
- Dart
- Firebase Auth
- Cloud Firestore
- Firebase Storage
- Google Sign-In
- AniList metadata search
- Android / Google Play Console

## What I built

This was a full app build from idea to Play Store release.

I handled:

- app planning and feature scope
- Flutter UI and navigation
- Firebase authentication
- Google Sign-In
- Firestore data modeling
- Firebase Storage cover uploads
- account and data deletion flows
- Play Store policy requirements
- closed testing feedback
- Android App Bundle release builds
- production launch prep

## Project structure

The production app uses a feature-based Flutter structure, roughly organized around:

- auth
- home dashboard
- manga collection
- shelves
- settings
- onboarding
- Firebase services
- theme control

The actual source code is kept private, but this repo documents the app, architecture, and product decisions.

## Key features

### Multi-shelf organization

Manga can be assigned to more than one shelf. This was added after testing because a single-shelf setup felt too limiting for real collections.

Example use cases:

- Currently Reading
- Shonen Jump
- Favorites
- Need to Complete
- Owned by Publisher

### Missing volume tracking

Users can track specific missing volume numbers, which makes the app useful while shopping or checking a collection.

### Metadata search

Users can search manga metadata to prefill fields like title, cover image, genre, publisher, and published volume count.

### Account and data controls

The app includes:

- email/password sign-up
- email verification
- Google Sign-In
- logout confirmation
- delete all app data
- delete account

## Challenges solved

### Moving from one shelf to multiple shelves

The original version supported one shelf per manga. After testing, I changed the model to support multiple shelf IDs while keeping backwards compatibility for older entries.

### Auth and account safety

I added email verification, Google Sign-In, session persistence handling, logout confirmation, and account deletion flows.

### Play Store readiness

I worked through release requirements including privacy policy, terms of service, data safety disclosures, account deletion links, signed app bundles, closed testing, and production release prep.

## What I learned

This project helped me get hands-on experience with:

- building a real Flutter app end-to-end
- designing Firebase-backed user data
- handling auth flows across email/password and Google Sign-In
- responding to tester feedback
- shipping through Google Play Console
- balancing feature ideas with realistic V1 scope

## Roadmap

Possible future improvements:

- barcode scanning
- import/export tools
- advanced collection stats
- wish list / hunting list improvements
- more theme options
- iOS support
- web companion version

## About

Manga Shelf is published under Bizarre Studios and built by Tyler Parrish.
