# Setup

**Add these four CLI tools that will help you in each step (needed)**

1. ### [Rename](https://pub.dev/packages/rename)
- add this library in `pubspec.yaml` rename: latest-version
- ```flutter pub global activate rename```

2. ### [Flutter_launcher_icons](https://pub.dev/packages/flutter_launcher_icons)
- add this library in `pubspec.yaml` flutter_launcher_icons: latest-version

3. ### [Flutterfire CLI](https://firebase.flutter.dev/docs/cli/)
- install [Node.js](https://nodejs.org/en/download)
- Run this command `npm install -g firebase-tools`
- ```dart pub global activate flutterfire_cli```

4. ### [Stacked CLI](https://stacked.filledstacks.com/docs/tooling/stacked-cli/)
- ```dart pub global activate stacked_cli```

## Initialize

Clone the ship app fast github repo

```bash
git clone https://github.com/MDSADABWASIM/ship-app-fast <your_app_name_here>
```

## Rename app packages and name (needed)

Run these commands one by one and replace your-app-name and your-bundle-id with your selected values: 
- ```rename setAppName --targets ios,android --value "your-app-name"```
- ```rename setBundleId --targets android --value "<your-bundle-id>" ex:"com.example.bundleId"```


## Change your app icons

- Replace your android icon on assets/icons/android_icon.png
- Replace your iOS icon on assets/icons/ios_icon.png
- `flutter pub get`
- `flutter pub run flutter_launcher_icons`

## Add Firebase in app (needed)
- ```flutterfire configure```
-   Import the generated file in main.dart  ```import 'firebase_options.dart';```

## If you want to use supabase instead of firebase
- Go to **[supabase](https://supabase.io/)** and create an account
- Create a new project
- Go to supbase dashboard and copy supabase url and public key(anon key) and paste it in your .env file(in codebase)

```
SUPABASE_PUBLIC_KEY = ''
SUPABASE_API_URL = ''
```

## To speed up development use Stacked CLI
-   **[Stacked](https://stacked.filledstacks.com)** is an MVVM based architecture that helps you to build your app faster.
-   You can create new services, views and viewModels with a single command.

?> For more use cases of `stacked-cli`, head over to the [stacked-cli documentation](https://stacked.filledstacks.com/docs/getting-started/overview)

## Setup is done, Let's start configuring your app

Go to **[Force update](force_update.md)** section.

