# simple_sensor

[![pub package](https://img.shields.io/pub/v/simple_sensor.svg)](https://pub.dev/packages/simple_sensor)

Flutter plugin for accessing the Android and iOS accelerometer, gyroscope, magnetometer and orientation sensors.

## Getting Started

To use this plugin, add `simple_sensor` as a [dependency in your pubspec.yaml
file](https://flutter.io/platform-plugins/).

```yaml
dependencies:
  simple_sensor: ^0.1.0
```

Import to your project.

``` dart
import 'package:simple_sensor/simple_sensor.dart';

motionSensors.magnetometer.listen((MagnetometerEvent event) {
    print(event);
});

```

## Screenshot

<img src="https://github.com/fettespferd/simple_sensor/raw/master/screenshot.png" width="30%" /># simple_sensor
