# Expo CLI Android Build Failure: Gradle Plugin Version Conflict

This repository demonstrates a bug encountered when building an Android app using the Expo CLI. The build process fails due to conflicts with the Android Gradle plugin version.  The error messages are often unclear, making debugging challenging.

## Bug Description

When attempting to build an Android APK using `expo build:android`, the build process terminates with an error related to the Gradle plugin version. This error may manifest in different ways depending on the project's dependencies and the current versions of the Expo CLI and Android Gradle Plugin.

## Reproduction

1. Clone this repository.
2. Navigate to the project directory.
3. Run `expo prebuild` and `expo build:android`.
4. Observe the build failure and error message.

## Solution

The solution involves carefully examining the error messages to identify the conflicting plugin versions.  This may require adjusting the `android/gradle/wrapper/gradle-wrapper.properties` file to specify a compatible Gradle version or modifying the project-level `build.gradle` file to resolve dependency conflicts.  In some cases, updating the Expo CLI to the latest version may also help resolve the issue.