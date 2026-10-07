# 05 - Components d'Android

## Activity

Una `Activity` representa una pantalla o punt d'interacció de l'aplicació.

## Service

Un `Service` permet executar determinades tasques que no depenen directament d'una interfície gràfica.

## Content Provider

Un `ContentProvider` proporciona una interfície per gestionar i compartir dades entre aplicacions quan el model de dades ho requereix.

## Broadcast Receiver

Un `BroadcastReceiver` permet reaccionar davant broadcasts generats pel sistema o per aplicacions.

## Notification Manager

Gestiona les notificacions que es presenten a l'usuari.

## View

En el sistema tradicional d'interfície Android, les `View` representen components visuals:

```text
TextView
Button
ImageView
EditText
```

En Android modern també és molt habitual **Jetpack Compose**.

## Resource Manager

Gestiona recursos com:

- imatges;
- sons;
- textos;
- colors;
- dimensions;
- icones.

## Intent

Un `Intent` permet comunicar-se entre components Android i iniciar determinades activitats o altres funcionalitats.

Exemple conceptual:

```text
Activity A
    |
  Intent
    |
    v
Activity B
```

## AndroidManifest.xml

El manifest declara informació essencial de l'aplicació, com:

- components;
- permisos;
- informació de compatibilitat;
- activitats;
- serveis;
- receivers;
- providers.
