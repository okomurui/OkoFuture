---
description: Overview
---

# Oko Future - General Technical Documentation

Oko Future is an iOS app that allows users to view 3D models and animations above physical clothes. The app is built using Swift 5 and Xcode 12. The app uses UIKit for the user interface, Combine for asynchronous programming, RealityKit and ARKit for augmented reality features, and AVFoundation for audio and video playback. The app follows the MVVM (Model-View-ViewModel) architecture pattern, with a router for navigation.

### Requirements

* Xcode 12 or higher
* Swift 5 or higher
* iOS 14 or higher
* A device with an A9 or later processor for ARKit support (iPhone X and newer)

### Installation

1. Run the app in the iOS simulator or on a physical device
2. Open `OkoFutureApp.xcodeproj` in Xcode
3. Clone the repository: `git clone` [`https://github.com/okofuture-app.git`](https://github.com/OkoFuture/OkoFuture.git)``

### Architecture

The app follows the MVVM (Model-View-ViewModel) architecture pattern:

* **Model:** The data model is defined using `RealityKit` and `ARKit`.
* **View:** The user interface is implemented using `UIKit` components.
* **ViewModel:** The app logic is implemented in `ViewModel` classes, which are responsible for handling data and business logic, and notifying the view when to update.
* **Router:** The app uses a router for navigation between views.

### Dependencies

The following libraries are used in the app:

* `Combine` for asynchronous programming
* `RealityKit` for 3D model rendering and animations
* `AVFoundation` for audio and video playback
* `ARKit` for augmented reality features
* `Metal` for 3D graphic and compute shader

### 3D Models and Animations

The app allows users to view 3D models and animations above physical clothes. The app uses `RealityKit` for rendering and animating 3D models. The 3D models are loaded from external `.usdz` files. As for reactive part we use Metal

### Augmented Reality

The app uses `ARKit` to track the user's device in real-world space and render 3D models and animations in a real-world environment. The app supports horizontal plane detection and anchors 3D models to real-world surfaces.

### Audio and Video Playback

The app uses `AVFoundation` to play audio and video files. The app supports playing audio and video files simultaneously with 3D model rendering and animation.

### Code Structure

The code is organized into the following directories:

* **Controllers:** Contains all `UIViewController` classes.
* **Models:** Contains all `RealityKit` and `ARKit` entities and data models.
* **Views:** Contains all `xib` and `storyboard` files.
* **ViewModels:** Contains all `ViewModel` classes for each view.
* **Routers:** Contains the router for navigation between views.
* **Utilities:** Contains helper classes and extensions.
* **Networking:** Contains classes for communicating with external APIs for 3D models and assets.

