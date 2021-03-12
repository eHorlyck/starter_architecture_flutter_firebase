# Starter Project
This is a fork of the [starter architecture](https://github.com/bizz84/starter_architecture_flutter_firebase) by Andrea

## Getting started
This section describes the steps neede to adapt this project.

### Mirror the starter repo

Create a new repository here on Github, without any readme.
```bash
git clone https://github.com/eHorlyck/starter_architecture_flutter_firebase.git
cd starter_architecture_flutter_firebase
```

Push mirror to the new repo
```bash
git push --mirror https://github.com/eHorlyck/NEW-REPOSITORY.git
```

Remove starter repo
```bash
cd ..
rm -rf starter_architecture_flutter_firebase
```

### Clone the new repository
```bash
git clone https://github.com/eHorlyck/NEW-REPOSITORY.git
cd NEW-REPOSITORY

```

### Rename the project and packages

Us the [Rename package](https://pub.dev/packages/rename)
```bash
# installing rename
flutter pub global activate rename

# Renaming the files
flutter pub global run rename --bundleId it.horlyck.APPNAME
flutter pub global run rename --appname "App Name"

# Remove this README.md and create new
rm README.md
touch README.md

# Commit all changes to Git
git commit -a -m "Renamed project"
```

### Open project to code to change package names
```bash
code .
```

search in all files (cmd + shif + f) for "com.example.starter_architecture_flutter_firebase" and relace with "it.horlyck.APPNAME"
The are in the following directories:
- android/app/src/debug/AndroidManifest.xml
- android/app/src/main/AndroidManifest.xml
- android/app/src/main/kotlin/com/example/starter_architecture_flutter_firebase/MainActivity.kt
- android/app/src/profile/AndroidManifest.xml

[Original Readme by Andrea](/Andreas-README.md)
