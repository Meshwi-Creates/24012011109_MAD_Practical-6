# Practical 6 – Frame by Frame Animation and Splash Screen

## Aim
Create an Android application to demonstrate frame-by-frame animation and splash screen with twin animation.

## Technologies Used
- Android Studio
- Kotlin
- XML
- Android SDK

## Description
This practical demonstrates frame-by-frame animation and splash screen animation in an Android application.

The application includes:
- Animated alarm images
- Animated heart
- Animated UVPCE logo
- Splash screen with gradient background
- Twin animation using translate, rotate and scale

## Features

### Splash Screen
- Displays the UVPCE logo with animation.
- Uses a radial gradient background.
- Applies twin animation to the logo.
- Opens the MainActivity after the animation is completed.

### Frame-by-Frame Animation
- Uses 10 alarm images to create a continuous animation.
- Uses multiple heart images to create a heart animation.
- `AnimationDrawable` is used to start the frame animations.

### Twin Animation
The splash screen uses:
- Translate animation
- Rotate animation
- Scale animation

These animations are combined using the `<set>` tag.

## Output

### Splash Screen
![Splash Screen](screenshots/splash_screen.png)

### Main Application
![Main Application](screenshots/main_screen.png)

## Project Structure

```text
app/
└── src/
    └── main/
        ├── java/
        │   └── MainActivity.kt
        │   └── SplashActivity.kt
        │
        ├── res/
        │   ├── anim/
        │   │   └── twinanimation.xml
        │   │
        │   ├── drawable/
        │   │   ├── alarm_animation_list.xml
        │   │   ├── heart_animation_list.xml
        │   │   ├── rectangular_gradiant.xml
        │   │   ├── alarm1 ... alarm10
        │   │   └── heart animation frames
        │   │
        │   └── layout/
        │       ├── activity_main.xml
        │       └── activity_splash.xml
        │
        └── AndroidManifest.xml
