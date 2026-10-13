# Lost and Found App

An Android app where users can report lost or found items, search through them and view full details. It was built in Java as a group semester project by students of the Information Technology department, and all data is stored locally on the phone using SQLite, so the app works fully offline.

## Project objectives

The main objectives of this project were to build an Android application that allows users to report lost or found items, give them an easy way to search for items, show contact details so the finder and the owner can reach each other, and keep the system simple and user friendly.

## Features

- User registration and login
- Add lost or found items with a title, description, location and contact number
- View all items in a list
- Search items by typing a keyword, which looks through the title, description and location
- Open any item to see its full details including the date and contact number
- Delete any item from the detail screen
- Works offline because all data is stored locally in SQLite

## Technologies used

### Java

Java is the main language of the app. The logic for registration, login, adding items, searching and deleting is written in Java, including the DatabaseHelper class that handles all database operations.

### SQLite

SQLite is used for local storage. There are two tables. The users table stores the user id, name, email and password. The items table stores the item id, title, description, location, date, contact number and the id of the user who added the item. All create, read and delete operations are done with SQL queries inside the DatabaseHelper class.

### XML

Every screen has its own XML layout file, such as the login, register, all items, add item and item detail screens. Custom colors and the app theme are defined in colors.xml, styles.xml and themes.xml.

### Android Studio and Gradle

The app was written and tested in Android Studio and built with Gradle. The minimum SDK is API 21 and the target SDK is API 33. No external libraries were needed because SQLite is already part of Android. It was tested on an emulator running Android 12 and on a physical phone running Android 13.

## How to run the project

1. Open the project in Android Studio.
2. Connect an Android phone with a USB cable or start an emulator running Android 5.0 or above.
3. Click the green Run button or press Shift + F10.
4. Wait for the app to install and then open it.
5. As a first time user, register with your full name, email and password.
6. Log in with the same email and password.
7. You can now add items, view all items, search and delete items.

## What is in this repository

The Android project is in the main folder. The docs folder has the project proposal and the full documentation.

## Why these technologies

We chose Java and SQLite because they are simple, well documented and do not need any paid license or cloud service. Since this was a semester project, we wanted something that works offline and is easy to demonstrate without internet.

## Limitations

This is a basic level app made for learning. The data stays only on the device and there is no cloud sync, so items added on one phone are not visible on another.

## What I learned

This project helped me understand how an Android app is planned and put together, how SQLite is used for local storage, and how a project moves from a proposal to working code and documentation.
