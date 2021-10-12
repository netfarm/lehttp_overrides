# lehttp_overrides

A Flutter package to solve SSL Certificate problem with Android 7 or earlier

## Getting Started

To resolve the issue linked to SSL Certificate, you need to add this line at the beginning of your
project:

```dart
import 'package:lehttp_overrides/lehttp_overrides.dart';

void main() {
  ...
  if (Platform.isAndroid){
    HttpOverrides.global = LEHttpOverrides();
  }
  ...
  runApp(const MyApp());
  }


```
