Camera4Kivy
===========

*Yet Another Camera for Kivy*

2023/02/09 : Android users: camerax_provider has been updated to version 0.0.3

- [Overview](https://github.com/Android-for-Python/Camera4Kivy#overview)
- [Install](https://github.com/Android-for-Python/Camera4Kivy#install)
  * [Install Camera4Kivy on Desktop](https://github.com/Android-for-Python/Camera4Kivy#install-camera4kivy-on-desktop)
  * [Install Camera4Kivy on Android](https://github.com/Android-for-Python/Camera4Kivy#install-camera4kivy-on-android)
    + [buildozer.spec:](https://github.com/Android-for-Python/Camera4Kivy#buildozerspec-)
    + [Run Time Permissions](https://github.com/Android-for-Python/Camera4Kivy#run-time-permissions)
  * [Install Camera4Kivy on iOS](https://github.com/Android-for-Python/Camera4Kivy#install-camera4kivy-on-ios)
    + [Run Time Permissions](https://github.com/Android-for-Python/Camera4Kivy#run-time-permissions-1)
- [Examples](https://github.com/Android-for-Python/Camera4Kivy#examples)
  * [Tested Examples](https://github.com/Android-for-Python/Camera4Kivy#tested-examples)
    + [C4K Photo Example](https://github.com/Android-for-Python/Camera4Kivy#c4k-photo-example)
    + [C4K QR Example](https://github.com/Android-for-Python/Camera4Kivy#c4k-qr-example)
    + [C4K OpenCV Example](https://github.com/Android-for-Python/Camera4Kivy#c4k-opencv-example)
    + [C4K MLKit Example](https://github.com/Android-for-Python/Camera4Kivy#c4k-mlkit-example)
    + [C4K TFLite Example](https://github.com/Android-for-Python/Camera4Kivy#c4k-tflite-example)
  * [Tested Platforms](https://github.com/Android-for-Python/Camera4Kivy#tested-platforms)
- [Preview Widget](https://github.com/Android-for-Python/Camera4Kivy#preview-widget)
  * [Preview Widget Properties](https://github.com/Android-for-Python/Camera4Kivy#preview-widget-properties)
    + [aspect_ratio](https://github.com/Android-for-Python/Camera4Kivy#aspect-ratio)
    + [letterbox_color](https://github.com/Android-for-Python/Camera4Kivy#letterbox-color)
    + [orientation](https://github.com/Android-for-Python/Camera4Kivy#orientation)
  * [Preview Widget API](https://github.com/Android-for-Python/Camera4Kivy#preview-widget-api)
    + [Connect Camera](https://github.com/Android-for-Python/Camera4Kivy#connect-camera)
      - [camera_id](https://github.com/Android-for-Python/Camera4Kivy#camera-id)
      - [mirrored](https://github.com/Android-for-Python/Camera4Kivy#mirrored)
      - [filepath_callback](https://github.com/Android-for-Python/Camera4Kivy#filepath_callback)
      - [sensor_resolution](https://github.com/Android-for-Python/Camera4Kivy#sensor_resolution)
      - [sensor_rotation](https://github.com/Android-for-Python/Camera4Kivy#sensor_rotation)
      - [default_zoom](https://github.com/Android-for-Python/Camera4Kivy#default_zoom)
      - [analyze_pixels_resolution](https://github.com/Android-for-Python/Camera4Kivy#analyze_pixels_resolution)
      - [enable_analyze_pixels](https://github.com/Android-for-Python/Camera4Kivy#enable_analyze_pixels)
      - [enable_analyze_imageproxy](https://github.com/Android-for-Python/Camera4Kivy#enable_analyze_imageproxy)
      - [enable_zoom_gesture](https://github.com/Android-for-Python/Camera4Kivy#enable_zoom_gesture)
      - [enable_focus_gesture](https://github.com/Android-for-Python/Camera4Kivy#enable_focus_gesture)
      - [imageproxy_data_format](https://github.com/Android-for-Python/Camera4Kivy#imageproxy_data_format)
    + [Disconnect Camera](https://github.com/Android-for-Python/Camera4Kivy#disconnect-camera)
    + [Capture](https://github.com/Android-for-Python/Camera4Kivy#capture)
      - [location](https://github.com/Android-for-Python/Camera4Kivy#location)
      - [subdir](https://github.com/Android-for-Python/Camera4Kivy#subdir)
      - [name](https://github.com/Android-for-Python/Camera4Kivy#name)
    + [Select Camera](https://github.com/Android-for-Python/Camera4Kivy#select-camera)
    + [Zoom](https://github.com/Android-for-Python/Camera4Kivy#zoom)
    + [Pan/scroll](https://github.com/Android-for-Python/Camera4Kivy#panscroll)
    + [Flash](https://github.com/Android-for-Python/Camera4Kivy#flash)
    + [Torch](https://github.com/Android-for-Python/Camera4Kivy#torch)
    + [Focus](https://github.com/Android-for-Python/Camera4Kivy#focus)
    + [camera_connected](https://github.com/Android-for-Python/Camera4Kivy#camera_connected)
- [Image analysis](https://github.com/Android-for-Python/Camera4Kivy#image-analysis)
  * [Overview and Examples](https://github.com/Android-for-Python/Camera4Kivy#overview-and-examples)
  * [User Interaction](https://github.com/Android-for-Python/Camera4Kivy#user-interaction)
  * [Coordinates and image encoding](https://github.com/Android-for-Python/Camera4Kivy#coordinates-and-image-encoding)
  * [Analysis Configuration](https://github.com/Android-for-Python/Camera4Kivy#analysis-configuration)
  * [Debugging](https://github.com/Android-for-Python/Camera4Kivy#debugging)
  * [Performance](https://github.com/Android-for-Python/Camera4Kivy#performance)
- [Camera Behavior](https://github.com/Android-for-Python/Camera4Kivy#camera-behavior)
  * [A Physical Camera](https://github.com/Android-for-Python/Camera4Kivy#a-physical-camera)
  * [Resolution](https://github.com/Android-for-Python/Camera4Kivy#resolution)
    + [Sensor Resolution](https://github.com/Android-for-Python/Camera4Kivy#sensor-resolution)
    + [Cropped Sensor Resolution](https://github.com/Android-for-Python/Camera4Kivy#cropped-sensor-resolution)
    + [Preview Resolution](https://github.com/Android-for-Python/Camera4Kivy#preview-resolution)
    + [Capture Resolution](https://github.com/Android-for-Python/Camera4Kivy#capture-resolution)
    + [Analysis Resolution](https://github.com/Android-for-Python/Camera4Kivy#analysis-resolution)
    + [Display Resolution.](https://github.com/Android-for-Python/Camera4Kivy#display-resolution)
- [Camera Provider](https://github.com/Android-for-Python/Camera4Kivy#camera-provider)
  * [Android Camera Provider](https://github.com/Android-for-Python/Camera4Kivy#android-camera-provider)
  * [OpenCV](https://github.com/Android-for-Python/Camera4Kivy#opencv)
  * [GStreamer](https://github.com/Android-for-Python/Camera4Kivy#gstreamer)
  * [Picamera](https://github.com/Android-for-Python/Camera4Kivy#picamera)
  * [AVFoundation](https://github.com/Android-for-Python/Camera4Kivy#avfoundation)
- [Known Behavior](https://github.com/Android-for-Python/Camera4Kivy#known-behavior)
  * [Behavior: Android .mp4 Orientation](https://github.com/Android-for-Python/Camera4Kivy#behavior-android-mp4-orientation)
  * [Behavior: Android .jpg Orientation.](https://github.com/Android-for-Python/Camera4Kivy#behavior-android-jpg-orientation)
  * [Behavior: Android armeabi-v7a build installed on an arm64-v8a device](https://github.com/Android-for-Python/Camera4Kivy#behavior-android-armeabi-v7a-build-installed-on-an-arm64-v8a-device)
  * [Behavior: Android "No supported surface combination"](https://github.com/Android-for-Python/Camera4Kivy#behavior-android-no-supported-surface-combination)
