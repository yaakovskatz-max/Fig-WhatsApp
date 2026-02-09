# Setup Guide for Signal Fork

## Introduction
This guide provides detailed instructions for building and installing the Signal fork as com.waze.

## Prerequisites
Before you start, ensure that you have the following installed:
- Java Development Kit (JDK)
- Android Studio
- Git
- Android SDK

## Clone the Repository
First, you need to clone the Signal fork repository:

```bash
git clone https://github.com/yourusername/Signal-Fork.git
cd Signal-Fork
```

## Build the Project
Open Android Studio and import the project:
1. Launch Android Studio.
2. Select `Open an existing Android Studio project`.
3. Navigate to the cloned repository and select it.

Build the project using the following Gradle command:

```bash
gradle build
```

## Modify Application ID
To set the application ID to com.waze, modify the following file:
- Open `build.gradle` located in the app directory.
  - Find the line that starts with `applicationId` and change its value to `com.waze`

## Install the APK
Once the build is successful, install the APK on your device with the following command:

```bash
adb install -r app/build/outputs/apk/debug/app-debug.apk
```

## Conclusion
You should now have the Signal fork installed as com.waze. If you encounter any issues, please refer to the documentation or seek help in the community.
