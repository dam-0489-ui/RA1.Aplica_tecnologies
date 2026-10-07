# Windows + Android Studio + Flutter/Dart

Guia per configurar Flutter/Dart a Windows utilitzant Android Studio.

## 1. Instal·lar Git

Descarregar Git per Windows i instal·lar-lo.

Comprovar des de PowerShell:

```powershell
git --version
```

## 2. Instal·lar Android Studio

Descarregar Android Studio per Windows.

Executar l'instal·lador `.exe` i seguir l'assistent.

Durant el primer inici, completar el Setup Wizard.

## 3. Configurar Android SDK

A Android Studio:

```text
Tools
-> SDK Manager
```

Comprovar:

- Android SDK Platform
- Android SDK Platform-Tools
- Android SDK Build-Tools
- Android SDK Command-line Tools
- Android Emulator

## 4. Crear emulador

```text
Tools
-> Device Manager
-> Create Virtual Device
```

Escollir un dispositiu, descarregar si cal la imatge del sistema i finalitzar.

Iniciar l'emulador.

## 5. Instal·lar Flutter

Descarregar el SDK estable de Flutter per Windows.

Crear una ubicació, per exemple:

```text
C:\srclutter
```

Descomprimir el ZIP de Flutter.

Evitar instal·lar-lo dins de `C:\Program Files` per no dependre de permisos d'administrador.

## 6. Afegir Flutter al PATH

Obrir:

```text
Configuració del sistema
-> Configuració avançada
-> Variables d'entorn
```

Editar el `Path` de l'usuari i afegir:

```text
C:\srclutterin
```

Tancar els terminals oberts i obrir un PowerShell nou.

## 7. Comprovar Flutter i Dart

```powershell
flutter --version
dart --version
```

Després:

```powershell
flutter doctor
```

## 8. Llicències Android

```powershell
flutter doctor --android-licenses
```

Acceptar les llicències quan es demani.

Tornar a executar:

```powershell
flutter doctor
```

## 9. Plugin Flutter a Android Studio

A:

```text
File
-> Settings
-> Plugins
-> Marketplace
```

buscar:

```text
Flutter
```

Instal·lar i reiniciar.

## 10. Crear projecte

```text
New Flutter Project
-> Flutter
```

Indicar el Flutter SDK:

```text
C:\srclutter
```

Indicar el nom del projecte i crear-lo.

## 11. Executar

Amb l'emulador iniciat:

```powershell
flutter devices
flutter run
```

També es pot executar des de Android Studio.

## 12. Mòbil físic

Activar:

- Opcions de desenvolupador
- Depuració USB

Connectar el dispositiu i comprovar:

```powershell
flutter devices
```

Executar:

```powershell
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
- [ ] `flutter doctor`
- [ ] Projecte executat
