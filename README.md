# simple_sensor

[![pub package](https://img.shields.io/pub/v/simple_sensor.svg)](https://pub.dev/packages/simple_sensor)

Flutter plugin for accessing the Android and iOS accelerometer, gyroscope, magnetometer and orientation sensors.

## Getting Started

To use this plugin, add `simple_sensor` as a [dependency in your pubspec.yaml
file](https://flutter.io/platform-plugins/).

```yaml
dependencies:
  simple_sensor: ^0.1.4
```

Import to your project.

``` dart
import 'package:simple_sensor/simple_sensor.dart';

## Sensor Events

This package provides access to various sensor events. Here's how you can use them:

### Accelerometer

The accelerometer measures the acceleration that the device is experiencing relative to freefall.

```dart
motionSensors.accelerometer.listen((AccelerometerEvent event) {
    print('X: ${event.x}');
    print('Y: ${event.y}');
    print('Z: ${event.z}');
});

Gyroscope
The gyroscope measures the rate or rotation in rad/s around each of the three axes.

motionSensors.gyroscope.listen((GyroscopeEvent event) {
    print('X: ${event.x}');
    print('Y: ${event.y}');
    print('Z: ${event.z}');
});

Magnetometer
The magnetometer measures the ambient geomagnetic field for all three physical axes (x, y, z) in μT.

motionSensors.magnetometer.listen((MagnetometerEvent event) {
    print('X: ${event.x}');
    print('Y: ${event.y}');
    print('Z: ${event.z}');
});

Absolute Orientation
The package also provides access to the absolute orientation of the device in terms of yaw, pitch, and roll.

motionSensors.absoluteOrientation.listen((AbsoluteOrientationEvent event) {
    print('Yaw: ${event.yaw}');
    print('Pitch: ${event.pitch}');
    print('Roll: ${event.roll}');
});
```

