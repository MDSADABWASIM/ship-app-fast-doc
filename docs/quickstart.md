# Quick start

Add these four CLI tools that will help you in each step (needed)

1. [rename](https://pub.dev/packages/rename)
- add this library in `pubspec.yaml` rename: latest-version
- ```flutter pub global activate rename```

2. [flutter_launcher_icons](https://pub.dev/packages/flutter_launcher_icons)
- add this library in `pubspec.yaml` flutter_launcher_icons: latest-version

3. [Flutterfire CLI](https://firebase.flutter.dev/docs/cli/)
- install [Node.js](https://nodejs.org/en/download)
- Run this command `npm install -g firebase-tools`
- ```dart pub global activate flutterfire_cli```

4. [Stacked CLI](https://stacked.filledstacks.com/docs/tooling/stacked-cli/)
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

## To speed up development use Stacked CLI
-   Example to create a new service: ```stacked create service onesignal```

?> For more use cases of `stacked-cli`, head over to the [stacked-cli documentation](https://stacked.filledstacks.com/docs/getting-started/overview)

