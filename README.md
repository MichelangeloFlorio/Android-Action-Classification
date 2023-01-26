# Esempio di applicazione di classificazione video basata su TensorFlow Lite

## Overview

This is an example application for
[TensorFlow Lite](https://tensorflow.org/lite) on Android. It uses
video classification to continuously classify whatever it sees from the device's back camera.
Inference is performed using the TensorFlow Lite Java API. The demo app
classifies frames in real-time, displaying the top most probable
classifications. It allows the user to choose between multiple variants of the [MoviNet](https://tfhub.dev/s?deployment-format=lite&q=movinet)
video classification model.

These instructions walk you through building and running the demo on an Android device.

### Model

We provide 3 integer-only quantized models bundled in this app:
* MoviNet-A0
* MoviNet-A1
* MoviNet-A2

MoviNet-A0 is the smallest and fastest model but less accurate than the A1 and A2. On the other 
hand, MoviNet-A2 is the most accurate one but also larger and slower.

Downloading, extracting, and placing the model in the assets folder is managed
automatically by download.gradle.

## Requirements

*   Android Studio Bumblebee | 2021.1.1 or newer (installed on a Linux, Mac or Windows machine)

*   Android device in
    [developer mode](https://developer.android.com/studio/debug/dev-options)
    with USB debugging enabled

*   USB cable (to connect Android device to your computer)

