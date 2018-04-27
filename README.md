### Quick Math - A gesture based math game for Android.

#### Introduction
QuickMath was developed as part of a fourth year module named Gesture Based UI Development. The idea was to create an educational game where users were able to solve Addition/Subtraction/Multiplication math equations with three different difficulties. The the math equations are dynamically generated based on game-mode and difficulty selected and the user uses their phone's microphone to answer the equations.

Successfully solving a mathematical equation rewards the user with a score point for their selected game - different difficulties provide more points per solve. The user can register/login using one input of a Username and a picture of their face.

The Android application was written using Ionic 3 with Native Camera and Native Speech assisted with Google Assist for speech recognition.

In this repository you will find the source code and APK for the application.

#### Architecture
The architecture of the application on the front end is based on Angular4 Components and Providers. There are two components: one for the authentication and the other for the game.

The providers supply the application with service-like functions. There are currently 3 providers: AuthProvider, ScoreProvider and SpeechProvider.

The AuthProvider supplies the login component with HTTP functions to contact the back-end for logging/registering a user.

The ScoreProvider supplies the game component with HTTP functions to contact the back-end for updating highscores.

Finally the SpeechProvider is used to supply the Game component with functions for acquiring permissions to use the microphone.

#### Gestures
##### Facial Recognition
Using the native camera on your android device, you can take a photo ID that acts as your password to the username. This enables the use of a facial gesture to authenticate users. We chose to do this gesture because it seems like this is a field of authentication that is being developed rapidly. It also acts as a fun-feature for kids to authenticate themselves with the help of their parents.

##### Voice Recognition
Using the native microphone on your android device and google assist Speech Recognition, you can record your answers to the math sums with a voice gesture.
