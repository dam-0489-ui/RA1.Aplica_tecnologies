# Ubuntu + Visual Studio Code + Flutter/Dart

Guia per configurar Flutter/Dart a Ubuntu utilitzant Visual Studio Code com a editor principal.

## 1. Preparar Ubuntu

```bash
sudo apt update
sudo apt upgrade -y
```

Instal·lar dependències:

```bash
sudo apt install -y curl git unzip xz-utils zip libglu1-mesa
```

## 2. Instal·lar Android Studio

Tot i utilitzar VS Code per programar, necessitem les eines Android.

Instal·lar Android Studio i, des de:

```text
Tools
-> SDK Manager
```

comprovar:

- Android SDK
- Android SDK Platform-Tools
- Android SDK Build-Tools
- Android SDK Command-line Tools
- Android Emulator

Crear també un dispositiu virtual des de:

```text
Tools
-> Device Manager
```

## 3. Instal·lar Flutter

Descarregar Flutter SDK.

```bash
mkdir -p ~/develop
tar -xf ~/Downloads/flutter_linux_*.tar.xz
```

Configurar el PATH:

```bash
echo 'export PATH="$HOME/develop/flutter/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Comprovar:

```bash
flutter --version
dart --version
```

## 4. Configurar Android

```bash
flutter doctor
```

Acceptar llicències:

```bash
flutter doctor --android-licenses
```

Tornar a comprovar:

```bash
flutter doctor
```

## 5. Instal·lar VS Code

Descarregar la versió oficial per Linux.

Si tenim un `.deb`:

```bash
cd ~/Downloads
sudo apt install ./code_*.deb
```

Comprovar:

```bash
code --version
```

## 6. Instal·lar Flutter a VS Code

Obrir VS Code:

```text
Extensions
-> Flutter
-> Install
```

La instal·lació de Flutter proporciona també la integració amb Dart.

## 7. Crear projecte

A VS Code:

```text
Ctrl + Shift + P
-> Flutter: New Project
-> Application
```

O des del terminal:

```bash
flutter create hola_flutter
cd hola_flutter
```

## 8. Executar

Iniciar l'emulador i comprovar:

```bash
flutter devices
```

Executar:

```bash
flutter run
```

També es pot utilitzar `F5` des de VS Code.

## 9. Checklist

- [ ] Git
- [ ] Android Studio per a les eines Android
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
