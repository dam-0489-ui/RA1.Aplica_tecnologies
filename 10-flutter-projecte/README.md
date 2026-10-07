# 10 - Estructura i primer projecte Flutter

## Crear un projecte

```bash
flutter create exemple
cd exemple
```

## Estructura

```text
exemple/
├── android/
├── ios/
├── lib/
│   └── main.dart
├── test/
├── web/
├── linux/
├── macos/
├── windows/
├── pubspec.yaml
└── ...
```

## `lib/`

Aquí escrivim habitualment el codi Dart de l'aplicació.

Exemple:

```text
lib/
├── main.dart
├── pantalla1.dart
├── pantalla2.dart
└── widgets/
```

## `pubspec.yaml`

Defineix la configuració del projecte i les dependències.

Exemple:

```yaml
dependencies:
  flutter:
    sdk: flutter
```

També permet declarar assets, fonts i paquets.

## Primer `main.dart`

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: const Text('Hola Flutter'),
        ),
        body: const Center(
          child: Text('Primera aplicació'),
        ),
      ),
    );
  }
}
```

## Executar

```bash
flutter devices
flutter run
```

## Comprovar el projecte

```bash
flutter analyze
```

I, si hi ha tests:

```bash
flutter test
```
