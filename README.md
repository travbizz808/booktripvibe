# BookTripVibe CRM Android App

Android WebView app for:

`https://booktripvibe.com/crm/login`

## Reference behavior

This project follows the supplied GoeARTH/GOAT CRM Android wrapper so BookTripVibe opens in the same app-style flow instead of a normal browser tab. The live BookTripVibe CRM remains the source of truth.

## Included

- Direct BookTripVibe CRM login launch
- Login cookies/session retained
- Mobile responsive WebView with normal mobile Chrome user-agent
- File upload support
- Standard downloads plus generated blob/data PDF download support
- Phone, email, intent and external-app links
- Android Back navigates CRM WebView history
- Network error panel with Retry
- Geolocation permission support for attendance/location features
- Cache cleared once after each Android app version update while login cookies remain intact
- BookTripVibe app name, package and brand colors

## Android configuration

- Package / Application ID: `com.booktripvibe.crm`
- Minimum Android: API 24 (Android 7.0)
- Target Android: API 35
- Version: `1.0.0`
- Start URL: `https://booktripvibe.com/crm/login`

## CRM files

The supplied BookTripVibe PHP CRM was inspected only to confirm its public CRM base/login route. No PHP/database functionality is required inside the Android project and the CRM archive itself was not modified for this wrapper.

## Build APK with GitHub Actions

1. Upload this Android project to the root of a GitHub repository.
2. Open **Actions** > **Build Android APK**.
3. Run the workflow.
4. Download artifact **BookTripVibe-CRM-APK**.
5. Extract `app-debug.apk`.

The workflow also runs on pushes to `main`.

## Main URL source

`app/src/main/java/com/booktripvibe/crm/MainActivity.java`
