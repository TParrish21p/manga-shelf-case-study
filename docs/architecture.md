# Architecture

Manga Shelf is built with Flutter and Firebase.

The app uses a feature-based structure so each main area of the app is easier to work on independently.

## Main areas

- Auth
- Home dashboard
- Manga collection
- Shelves
- Settings
- Onboarding
- Theme control
- Firebase services

## Backend

Firebase is used for:

- user authentication
- Google Sign-In support
- manga collection data
- shelf data
- uploaded cover images

## Data model overview

Each user has their own private data space.

Main user-owned data includes:

- manga entries
- shelves
- uploaded cover references
- notes and collection metadata

Manga entries support multiple shelf IDs so a single series can appear on more than one shelf.
