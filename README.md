# TaskFlow-app: Todo Task Management Mobile Application

![App Screenshot Placeholder](https://github.com/alireza4585/flutter-to-do-app/assets/102475069/ac08ec28-560f-4bc6-a728-026c9556e1f4)
*(Note: The above image is a placeholder. A screenshot/GIF of the actual working app will be updated here upon completion.)*

## Overview

This project is a cross-platform Todo Task Management Mobile Application developed for the Katomaran Hackathon. It aims to provide users with a seamless and intuitive experience for managing their personal tasks on the go, featuring social login, full CRUD operations on tasks, and real-time data synchronization.

## Tutorial / Demo Video

A detailed explanation and demonstration of the working application will be available here.
**Loom Video Link:** [Will be updated here upon submission]

## Features

* **User Authentication:** Secure user registration and login using Google Sign-In, powered by Firebase Authentication.
* **Real-time Task Management:**
    * **Create:** Easily add new tasks with a title, description, and due date.
    * **Read (List):** View all tasks, with options for filtering and searching.
    * **Update:** Modify existing tasks.
    * **Mark as Complete:** Visually indicate completed tasks.
    * **Delete:** Remove tasks no longer needed.
* **Intuitive User Experience:**
    * Clean, responsive UI designed for both Android and iOS.
    * Intuitive UI components including tabs (for task categories/filters), search functionality, and a Floating Action Button (FAB) for adding new tasks.
    * Clear "No data" states when no tasks are present.
    * Smooth animations for list interactions (e.g., task insertion, deletion, completion).
    * Pull-to-refresh functionality for task lists.
    * Swipe-to-delete gesture for quick task removal.
* **Offline Support:** Tasks are stored locally for session persistence, ensuring basic functionality even without an internet connection. Data is synchronized with the backend once connectivity is restored.
* **Crash Reporting:** Integrated with Firebase Crashlytics for real-time crash monitoring and reporting.

## Tech Stack

* **Mobile App Framework:** Flutter
* **Backend & Authentication:** Firebase (Authentication, Firestore)
* **Authentication Provider:** Google Sign-In

## Scope & Requirements Fulfilled

### 1. Onboarding & Authentication
* Implemented social login flow using **Google Sign-In** via Firebase Authentication.
* Appropriate error states are shown on login failure.

### 2. Task Management
* Supports full in-app CRUD operations: Create, Read (List), Update, Mark as Complete, and Delete tasks.
* Task fields include: title, description, due date, and status (open/complete).
* Task data is stored in Firebase Firestore for real-time sync and also managed in local state for the session.

### 3. User Experience
* Utilizes intuitive UI components:
    * Tabs for filtering tasks (e.g., "All," "Completed," "Pending").
    * Search functionality to quickly find tasks.
    * Clear "No data" states when there are no tasks to show.
    * A Floating Action Button (FAB) is used for adding new tasks.
* Smooth animations are implemented for list interactions (e.g., insertion, deletion, completion).

### 4. Polish & Extras
* Implemented pull-to-refresh for task lists.
* Implemented swipe-to-delete for better UX.
* Integrated crash reporting using Firebase Crashlytics.

## Assumptions Made

* **Backend Choice:** Firebase Firestore is assumed for the backend database due to its real-time capabilities and seamless integration with Flutter and Firebase Authentication.
* **Authentication Provider:** Google Sign-In was chosen as the primary social login provider for simplicity and widespread use.
* **Offline Support Implementation:** Offline support is handled by Firebase Firestore's built-in offline capabilities, which cache data locally and synchronize when online.
* **Task Priority:** While "priority" was mentioned as a field, for the hackathon scope, tasks are not explicitly prioritized beyond their due date and status. This can be extended in future iterations.
* **Task Categories:** Tasks can be conceptually organized by filters (e.g., "Completed", "Pending"), which serves as a basic form of categorization. More advanced, user-defined categories could be added.

## Architecture Diagram

*(An architecture diagram illustrating the app's components, data flow, and interaction with Firebase services will be attached with the submission.)*

## Setup Instructions

Follow these steps to get the TaskFlow-app running on your local machine.

### Prerequisites

* [Flutter SDK](https://flutter.dev/docs/get-started/install) (version 3.32.5 or higher recommended)
* [Android Studio](https://developer.android.com/studio) (for Android SDK and emulator setup)
* [VS Code](https://code.visualstudio.com/) (or your preferred IDE)
* A Firebase project set up with Authentication (Google Sign-In enabled) and Firestore Database.

