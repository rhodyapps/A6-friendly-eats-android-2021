# Friendly Eats

Branch: Step 4 Set up the Firebase emulators
previous steps:
- clone the repo: git clone https://github.com/firebase/friendlyeats-android
- Create a new firebase project 'friendlyeats-android'
- add android app package name: com.google.firebase.example.fireeats
- download google-services.json file and copy it to the 'app' folder

In this codelab you'll use the Firebase Emulator Suite to locally emulate Cloud Firestore and other Firebase services. This provides a safe, fast, and free local development environment to build your app.

In Android Studio:
- import the project (Use the second option under the three vertical dots on the screen that lists recent projects). Navigate to the project folder on your machine and click 'open'.

- open a new terminal and run the command: npm install -g firebase-tools
if you get EACCESS errors run the same command again but include 'sudo' (Super User DO):
sudo npm install -g firebase-tools

- Check that firebase is installed: firebase --version (it should return a version number)
- run: firebase login 

- run: firebase use --add
Select the project and enter an alias name either 'default' or 'friendlyeats-android'

- Run the emulators: 
In your terminal from within the friendlyeats-android directory run firebase emulators:start to start up the Firebase Emulators.

CodeLab Step 5 'Run the App'

Run the App in the Android Emulator in Android Studio:

- Click: Build > Rebuild Project 
- Click: Run
The Android emulator should start after the build is finished. Use the 'Build' tab at the bottom of Android Studio to see the build progress.
Use LogCat to see the messages between the Android Emulator and Android Studio


################ CODELAB DOCUMENTATION ################

This is the source code that accompanies the Firestore Android Codelab:
https://codelabs.developers.google.com/codelabs/firestore-android

The codelab will walk you through developing an Android restaurant recommendation
app powered by Cloud Firestore.

<img src="docs/home.png" width="300"/>

If you don't want to do the codelab and would rather view the completed
sample code, see the Firebase Android Quickstart repository:
https://github.com/firebase/quickstart-android

## Build Status

[![Actions Status][gh-actions-badge]][gh-actions]

[gh-actions]: https://github.com/firebase/friendlyeats-android/actions
[gh-actions-badge]: https://github.com/firebase/friendlyeats-android/workflows/Android%20CI/badge.svg
