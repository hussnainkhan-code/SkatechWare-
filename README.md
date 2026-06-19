# SkatechWare - Android Application

![SkatechWare](https://img.shields.io/badge/SkatechWare-1.0-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Android](https://img.shields.io/badge/Android-21%2B-brightgreen)

## Overview
SkatechWare is a modern Android application built with the latest Android development practices and technologies.

## Features
✅ Modern Material Design UI
✅ MVVM Architecture
✅ Retrofit for API Integration
✅ Room Database Support
✅ Coroutines for Asynchronous Operations
✅ Data Binding
✅ Comprehensive Testing

## Project Structure
```
SkatechWare/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/skatechware/app/
│   │   │   │   ├── api/              (API related classes)
│   │   │   │   ├── model/            (Data models)
│   │   │   │   ├── ui/               (UI activities & fragments)
│   │   │   │   ├── util/             (Utility classes)
│   │   │   │   └── MainActivity.java
│   │   │   ├── res/
│   │   │   │   ├── layout/           (XML layouts)
│   │   │   │   ├── values/           (Resources)
│   │   │   │   └── xml/              (XML configuration)
│   │   │   └── AndroidManifest.xml
│   │   ├── test/                     (Unit tests)
│   │   └── androidTest/              (Instrumented tests)
│   ├── build.gradle
│   └── proguard-rules.pro
├── build.gradle
├── settings.gradle
├── gradle.properties
└── README.md
```

## Requirements
- Android SDK 21 or higher
- Java 11 or higher
- Gradle 8.0.0 or higher

## Building the APK

### Prerequisites
1. Clone the repository
2. Open the project in Android Studio
3. Sync Gradle files

### Build Commands

**Debug APK:**
```bash
./gradlew assembleDebug
```

**Release APK:**
```bash
./gradlew assembleRelease
```

**Using the build script:**
```bash
chmod +x build-apk.sh
./build-apk.sh
```

## Output Locations
- **Debug APK:** `app/build/outputs/apk/debug/app-debug.apk`
- **Release APK:** `app/build/outputs/apk/release/app-release.apk`

## Dependencies
- AndroidX AppCompat
- Material Components
- Retrofit 2
- OkHttp 3
- Room Database
- Glide Image Loading
- Kotlin Coroutines
- Lifecycle Components

## Key Classes

### MainActivity
Main entry point of the application with Material Design UI.

### PreferenceManager
Utility class for managing SharedPreferences.

### NetworkUtils
Helper class for network connectivity checks.

### Logger
Centralized logging utility.

### RetrofitClient
Retrofit HTTP client configuration.

### User Model
Data model for user objects.

## Installation
```bash
adb install app/build/outputs/apk/debug/app-debug.apk
```

## Configuration

### API Configuration
Edit `RetrofitClient.java` to change the base URL:
```java
private static final String BASE_URL = "https://api.example.com/";
```

### App Branding
Update resources in `res/values/` to customize app name, colors, and strings.

## Testing
Run unit tests:
```bash
./gradlew test
```

Run instrumented tests:
```bash
./gradlew connectedAndroidTest
```

## Build Features
- ✅ View Binding
- ✅ Data Binding
- ✅ ProGuard Code Obfuscation
- ✅ Multi-APK Support

## Troubleshooting

**Build fails with Gradle error:**
```bash
./gradlew clean build
```

**SDK not found:**
Update your local SDK path in `local.properties`

**Permission issues:**
Ensure all required permissions are declared in `AndroidManifest.xml`

## Development Tools
- Android Studio (recommended)
- Git for version control
- Gradle for build automation

## Code Quality
- Unit tests included
- Instrumented tests included
- ProGuard rules configured
- Logging utilities provided

## Security
- Network requests use HTTPS
- SharedPreferences for secure storage
- Input validation implemented
- No hardcoded credentials

## Support
For issues and feature requests, please check the documentation or contact support.

## License
This project is licensed under the MIT License - see LICENSE file for details.

## Author
SkatechWare Development Team

## Version
1.0.0

---

**Built with ❤️ using Android Studio and Modern Android Development Practices**
