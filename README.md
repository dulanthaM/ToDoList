# Native To-Do List App Documentation

## 1. Introduction

This document provides an overview of the Native To-Do List App developed using Android Studio with SQLite for Android 6.0 and above.

## 2. Setting Up the App

1. Clone the repository.
2. Open the project in Android Studio.
3. Build and run on an emulator or a physical device.

## 3. Code Structure

The codebase for the Native To-Do List App is organized following standard Android application development practices. Below is an overview of the primary components and their roles within the code structure:

### 1. Activities

- **MainActivity.java:**
  - Central activity responsible for initializing the app.
  - Manages the UI, RecyclerView setup, and user interactions.
  - Integrates the ToDoAdapter for handling task list display.

- **SplashActivity2.java:**
  - Splash screen activity displaying the app logo.
  - Transitions to the main activity after a short delay.

- **AddNewTask.java:**
  - Bottom sheet dialog fragment for adding or editing tasks.
  - Implements the DialogCloseListener interface for task list updates.

### 2. Adapters

- **ToDoAdapter.java:**
  - RecyclerView adapter for managing task items.
  - Integrates with the DatabaseHandler for data operations.
  - Facilitates task deletion, editing, and status updates.

### 3. Database Handling

- **DatabaseHandler.java:**
  - Class that is a standard class used for database handling in the industry.
  - SQLiteOpenHelper class managing database creation, opening, and CRUD operations.
  - Configures the database with constants for version, name, and table details.
  - Implements methods for inserting, retrieving, updating, and deleting tasks.

### 4. Utilities

- **RecyclerItemTouchHelper.java:**
  - Helper class extending ItemTouchHelper.SimpleCallback.
  - Manages swipe gestures on RecyclerView items for delete and edit actions.
