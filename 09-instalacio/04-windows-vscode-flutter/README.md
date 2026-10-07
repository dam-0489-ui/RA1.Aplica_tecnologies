# Windows + Visual Studio Code + Flutter/Dart

Guia per configurar Flutter/Dart a Windows utilitzant Visual Studio Code.

## 1. Instal·lar Git

Instal·lar Git per Windows.

Comprovar:

```powershell
git --version
```

## 2. Instal·lar Android Studio

Encara que utilitzarem VS Code per programar, Android Studio és útil i necessari per disposar de les eines Android.

Instal·lar Android Studio i configurar:

```text
Android SDK
Android SDK Platform-Tools
Android SDK Build-Tools
Android SDK Command-line Tools
Android Emulator
```

Crear un dispositiu virtual des de:

```text
Tools
-> Device Manager
```

## 3. Instal·lar Flutter

Descarregar Flutter SDK per Windows.

Per exemple:

```text
C:\srclutter
```

Descomprimir-hi el SDK.

## 4. PATH

Afegir:

```text
C:\srclutterin
```

al `Path` de les variables d'entorn de l'usuari.

Obrir un PowerShell nou.

Comprovar:

```powershell
flutter --version
dart --version
```

## 5. Configurar Android

Executar:

```powershell
flutter doctor
```

Acceptar llicències:

```powershell
flutter doctor --android-licenses
```

Tornar a comprovar:

```powershell
flutter doctor
```

## 6. Instal·lar Visual Studio Code

Descarregar VS Code per Windows.

La instal·lació User Setup és una opció adequada per a la majoria d'usuaris.

## 7. Instal·lar Flutter/Dart

A VS Code:

```text
Extensions
-> Flutter
-> Install
```

L'extensió Flutter proporciona també la integració amb Dart.

## 8. Crear projecte

Obrir:

```text
Ctrl + Shift + P
```

Seleccionar:

```text
Flutter: New Project
-> Application
```

Escollir una carpeta i indicar el nom del projecte.

## 9. Alternativa amb terminal

```powershell
flutter create hola_flutter
cd hola_flutter
```

## 10. Executar

Iniciar l'emulador Android.

Comprovar:

```powershell
flutter devices
```

Executar:

```powershell
flutter run
```

O utilitzar:

```text
F5
```

## 11. Mòbil físic

Activar la depuració USB al dispositiu Android.

Comprovar:

```powershell
flutter devices
```

I executar:

```powershell
flutter run
```

## 12. Checklist

- [ ] Git
- [ ] Android Studio
- [ ] Android SDK
- [ ] Emulator
- [ ] Flutter SDK
- [ ] PATH
- [ ] Llicències
- [ ] VS Code
- [ ] Flutter extension
- [ ] Dart
- [ ] `flutter doctor`
- [ ] Projecte executat
