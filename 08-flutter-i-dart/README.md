# 08 - Flutter i Dart

## Què és Flutter?

Flutter és un framework multiplataforma que permet construir interfícies i aplicacions per a diverses plataformes.

## Què és Dart?

Dart és el llenguatge utilitzat per Flutter.

Exemple:

```dart
void main() {
  print('Hola Flutter!');
}
```

## Flutter no és l'IDE

Cal diferenciar:

```text
Dart
  -> llenguatge

Flutter
  -> framework + SDK

Android Studio
  -> IDE

Visual Studio Code
  -> editor/IDE extensible
```

## Plataformes

Flutter pot treballar amb:

- Android
- iOS
- Web
- Windows
- Linux
- macOS

## Flutter + Android Studio

```text
Android Studio
+
Flutter SDK
+
Flutter plugin
+
Dart
+
Android SDK
```

## Flutter + Visual Studio Code

```text
Visual Studio Code
+
Flutter extension
+
Dart extension
+
Flutter SDK
```

## Avantatge principal

Una gran part del codi es pot compartir entre plataformes.

```text
                 Flutter
                    |
       +------------+------------+
       |            |            |
    Android        iOS          Web
```

Això no significa que les plataformes siguin idèntiques: quan cal, Flutter pot integrar funcionalitats específiques natives.
