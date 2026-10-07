# 07 - Kotlin vs. Swift/iOS

## Kotlin i Android

Kotlin és el llenguatge principal del desenvolupament Android modern.

Exemple:

```kotlin
fun saludar(nom: String): String {
    return "Hola $nom"
}
```

Entorn habitual:

```text
Kotlin
+
Android Studio
+
Android SDK
+
Jetpack
```

## Swift i iOS

Swift és el llenguatge principal de desenvolupament de les plataformes Apple.

Exemple:

```swift
func saludar(nom: String) -> String {
    return "Hola \(nom)"
}
```

Entorn habitual:

```text
Swift
+
Xcode
+
iOS SDK
+
SwiftUI / UIKit
```

## Comparativa

| Aspecte | Kotlin / Android | Swift / iOS |
|---|---|---|
| Llenguatge | Kotlin | Swift |
| IDE | Android Studio | Xcode |
| SDK | Android SDK | iOS SDK |
| UI moderna | Jetpack Compose | SwiftUI |
| UI tradicional | Views/XML | UIKit |
| Hardware | Diversos fabricants | Ecosistema Apple |
| Distribució principal | Google Play | App Store |
| Desenvolupament natiu | Android | Plataformes Apple |

## Idea clau

Kotlin i Swift són alternatives **natives** de plataformes diferents.

Flutter/Dart és una alternativa **multiplataforma**:

```text
Dart + Flutter
       |
       +-- Android
       +-- iOS
       +-- Web
       +-- Desktop
```
