# Ubuntu + Android Studio + Flutter/Dart

Guia per preparar des de zero un entorn Flutter/Dart orientat a Android utilitzant Ubuntu i Android Studio.

## 1. Actualitzar Ubuntu

```bash
sudo apt update
sudo apt upgrade -y
```

## 2. Instal·lar dependències

```bash
sudo apt install -y curl git unzip xz-utils zip libglu1-mesa
```

Comprovar:

```bash
git --version
curl --version
```

## 3. Instal·lar Android Studio

Descarregar Android Studio des de la pàgina oficial d'Android.

Per Linux es pot descarregar l'arxiu `.tar.gz`.

Crear una carpeta:

```bash
mkdir -p ~/apps
```

Anar a Descàrregues:

```bash
cd ~/Downloads
```

Descomprimir:

```bash
tar -xzf android-studio-*.tar.gz
```

Moure:

```bash
mv android-studio ~/apps/
```

Executar:

```bash
~/apps/android-studio/bin/studio
```

Durant el primer inici, seguir el Setup Wizard.

## 4. Configurar Android SDK

A Android Studio:

```text
Tools
-> SDK Manager
```

Comprovar especialment:

- Android SDK Platform
- Android SDK Platform-Tools
- Android SDK Build-Tools
- Android SDK Command-line Tools
- Android Emulator

## 5. Crear un emulador

A Android Studio:

```text
Tools
-> Device Manager
-> Create Virtual Device
```

Seleccionar un dispositiu, una imatge Android i finalitzar.

Iniciar-lo amb el botó de reproducció.

## 6. Instal·lar Flutter

Descarregar el SDK estable de Flutter.

Crear una carpeta:

```bash
mkdir -p ~/develop
```

Descomprimir el SDK:

```bash
tar -xf ~/Downloads/flutter_linux_*.tar.xz
```

El resultat hauria de ser:

```text
~/develop/flutter
```

## 7. Configurar el PATH

Per Bash:

```bash
echo 'export PATH="$HOME/develop/flutter/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Comprovar:

```bash
flutter --version
dart --version
```

## 8. Configurar Android per Flutter

Executar:

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

## 9. Instal·lar Flutter a Android Studio

A Android Studio:

```text
File
-> Settings
-> Plugins
-> Marketplace
```

Buscar:

```text
Flutter
```

Instal·lar el plugin i reiniciar Android Studio.

## 10. Crear un projecte

Seleccionar:

```text
New Flutter Project
-> Flutter
```

Indicar el Flutter SDK, el nom del projecte i crear-lo.

## 11. Executar

Amb l'emulador iniciat:

```bash
flutter devices
flutter run
```

També es pot executar amb el botó Run de l'IDE.

## 12. Provar amb un mòbil físic

Activar al dispositiu:

- Opcions de desenvolupador
- Depuració USB

Connectar-lo i comprovar:

```bash
flutter devices
```

Després:

```bash
flutter run
```

## 13. Checklist

- [ ] Git
- [ ] Android Studio
- [ ] Android SDK
- [ ] Command-line Tools
- [ ] Emulator
- [ ] Flutter SDK
- [ ] PATH
- [ ] Llicències
- [ ] Flutter plugin
- [ ] `flutter doctor` correcte
- [ ] Projecte executat
