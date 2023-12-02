# hive

## Description

A Chat System Mobile Application Called Hive

## Table of Contents

- [Project Structure](#project-structure)
- [Activities](#activities)
  - [LoaderActivity](#loaderactivity)
  - [MainActivity](#mainactivity)
  - [SignInActivity](#signinactivity)
  - [SignUpActivity](#signupactivity)
- [Permissions](#permissions)
- [Manifest](#manifest)

## Project Structure

```
/app
|-- /src
    |-- /main
        |-- /java
            |-- /com.example.hive
                |-- /activities
                    |-- LoaderActivity.java
                    |-- MainActivity.java
                    |-- SignInActivity.java
                    |-- SignUpActivity.java
                |-- /firebase
                    |-- MessagingService.java
                |-- /utilities
                    |-- Constants.java
                    |-- PreferenceManager.java
        |-- /res
        |-- AndroidManifest.xml
```

## Activities

### LoaderActivity

The `LoaderActivity` serves as the launcher activity. It displays a loading screen and redirects the user to the `SignInActivity` after a delay.

### MainActivity

The `MainActivity` is the main activity of the application. Describe its purpose and functionality.

### SignInActivity

The `SignInActivity` allows users to sign in. It includes form validation and communicates with Firebase Firestore for authentication.

### SignUpActivity

The `SignUpActivity` facilitates user registration. It includes image selection from the gallery and communicates with Firebase Firestore for user creation.

## Permissions

Permissions required by this application.

- `INTERNET`: Used for network communication.
- `READ_EXTERNAL_STORAGE`: Needed for reading images from the gallery.
- `MANAGE_EXTERNAL_STORAGE`: Required for managing external storage on Android 11 and above.
- `READ_MEDIA_VIDEO`, `READ_MEDIA_AUDIO`, `READ_MEDIA_IMAGES`: Specific media-related permissions.

## Manifest

Elements in the AndroidManifest.xml file.

- `<uses-permission>`: Specifies required permissions.
- `<application>`: Configures application-wide settings.
- `<activity>`: Defines each activity, including the launcher (`LoaderActivity`), sign-in, sign-up, and main activities.
- `<service>`: Describes the messaging service for Firebase Cloud Messaging.

