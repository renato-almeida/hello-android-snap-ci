[![Build Status](https://snap-ci.com/renato-almeida/hello-android-snap-ci/branch/master/build_image)](https://snap-ci.com/renato-almeida/hello-android-snap-ci/branch/master)

# Hello Android Snap-CI
Simple test to try the [Snap-CI](http://snap-ci.com) platform


#Objective
The objective was to play a bit with the Snap-CI platform, to see the features and possibilities.
The app doesn't have anything special, it was the default one created by Android Studio :D 

I've created a pipeline with several steps/stages:
- Setup
  - Download Android build tools, platforam, emulators and other stuff
- Assemble `./gradlew assemble`
  - Simply compile the project to see if there are any errors 
- Unit Tests `./gradlew test`
  - Run unit tests 
- UI Tests `./gradlew connectedAndroidTest`
  - Run automatic tests (currently not working because on an error, GLIBC_2.15 not found)

##TODO
- Create a script to use on Setup stage
- Add script to download selected build tools, platform and emulator
