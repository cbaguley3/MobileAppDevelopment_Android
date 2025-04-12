Snowflake Vacation Manager Android Application

## Overview

This project involves developing an Android mobile application for managing vacations and excursions. It builds upon concepts similar to the D287 project but implemented for a mobile platform. The application allows users to manage vacation details (including start and end dates, hotel name, alerts, and sharing) and associated excursions (including date and alerts with date validation).

## Technologies Used

### Mobile Development

* Java (for application logic)
* Android SDK (for building Android applications)
* Android Studio (Integrated Development Environment)
* Gradle (build automation tool)
* Groovy (for Gradle build scripts)
* XML (for layout definitions)
* Room Persistence Library (for local data storage and interaction)
* ViewModel and LiveData (for managing UI-related data in a lifecycle-conscious way)
* Intent (for inter-component communication)
* AlarmManager (for scheduling alerts)
* ShareCompat.IntentBuilder (for sharing functionality)

### Development Environment & Tools

* Android Studio
* Git
* GitLab (for version control and CI/CD pipeline)
* Canva (optional, for storyboard creation)

## Feature Implementation

### Task A: GitLab Pipeline

* Successfully ran the CI/CD pipeline for the provided GitLab repository.

### Tasks B & C: Core Application Structure

* Developed the basic structure of the Android application, adapting the bicycle shop example from the webinars to a vacations and excursions management app.
* Replaced the "price" attribute with a "hotel name" (String) in the Vacation entity and related files (adapters, details, list).
* Created entities for Vacation and Excursion with relevant attributes (including start and end dates for Vacation, and date for Excursion).
* Implemented Room database integration (`AppDatabase`, DAOs, Entities).
* Developed UI layouts (`XML`) for vacation and excursion lists and details pages.
* Implemented adapters (`RecyclerView.Adapter`) to display lists of vacations and excursions.
* Implemented functionality to add, view, update, and delete vacations and excursions.
* Potentially implemented programmatic database clearing for development purposes.

### Additional Features (Beyond Basic Structure)

* **Vacation Details:**
    * Added start and end dates to the Vacation entity and UI.
    * Implemented the ability to set an alert for a vacation using `AlarmManager`.
    * Implemented the ability to share vacation details using `ShareCompat.IntentBuilder`.
* **Excursion Details:**
    * Added a date to the Excursion entity and UI.
    * Implemented the ability to set an alert for an excursion using `AlarmManager`.
    * Implemented date validation to prevent creating excursions before the vacation start date or after the vacation end date.
    * Added a "Delete Excursion" option to the toolbar on the excursion details page.
* **Validation:**
    * Implemented validation in the Vacation Details screen to prevent setting an end date before the start date.
    * Implemented validation in the Excursion Details screen to ensure the excursion date falls within the vacation's start and end dates.

### Task D: Storyboard

* Created a simple storyboard using Canva (or a similar tool) depicting the user interface flow from the home screen to all other screens of the application.
* Exported the storyboard as a PNG file.

### Task E: Signed APK

* Followed the webinar instructions to build a signed APK of the application.
* Included screenshots of the signed APK generation process and the resulting files.
* Noted the Android version used for testing (either on a physical device or emulator).

## Setup

1. Download and install Android Studio.
2. Clone the GitLab repository for the project.
3. Open the project in Android Studio.
4. Ensure the Android SDK is configured correctly.
5. Build and run the application on an Android emulator or a physical Android device (with USB debugging enabled).

## Git Repository

* **Repository URL:** https://github.com/cbaguley3/MobileAppDevelopment_Android/new/master
* **Branch:** master

## Commit History (Relevant to described features)

* Initial project setup and GitLab pipeline configuration.
* Implemented core vacation and excursion management features.
* Added hotel name instead of price.
* Implemented start and end dates for vacations.
* Implemented date for excursions.
* Implemented vacation alert functionality.
* Implemented excursion alert functionality with date validation.
* Implemented vacation end date validation.
* Implemented sharing functionality for vacations.
* Added delete excursion option.
* Created storyboard.
* Built and signed APK.
* Created and updated README file.
