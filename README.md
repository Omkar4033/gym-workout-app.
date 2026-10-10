# Gym Workout Plan (Android)

An offline Android app that wraps the workout guide: six-day plan, a figure and a photo for every
exercise, target muscles, set-by-set notes, three alternatives per exercise, and a gym-day calendar.
No internet permission; the calendar is stored on the phone.

## Build with Android Studio

1. Install Android Studio and open this folder (`File > Open`).
2. Wait for the Gradle sync to finish (first time downloads Gradle and the Android plugin).
3. `Build > Build App Bundle(s) / APK(s) > Build APK(s)`.
4. The file is `app/build/outputs/apk/debug/app-debug.apk`. Copy it to the phone and open it to install.
   Or connect the phone with USB debugging on and press Run.

## Build with GitHub Actions (no Android Studio)

1. Push this folder to a GitHub repository (branch `main`).
2. Open the repository's Actions tab and wait for "Build APK" to finish.
3. Download the `GymWorkoutPlan-apk` artifact, unzip it, and install `app-debug.apk` on the phone.

## Command line

`./gradlew assembleDebug` (needs JDK 17 and the Android SDK, platform 34).

## Where things are

- `app/src/main/assets/index.html`: the whole app (HTML, CSS, JavaScript, fonts).
- `app/src/main/assets/img/`: exercise photos.
- `app/src/main/java/.../MainActivity.java`: the WebView shell.

## Credits

Photos: Free Exercise DB (public domain, Unlicense). Fonts: Barlow and Barlow Condensed (SIL Open Font License).
