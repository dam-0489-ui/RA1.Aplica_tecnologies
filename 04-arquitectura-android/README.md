# 04 - Arquitectura d'Android

Android presenta una arquitectura formada per diverses capes.

```text
+-----------------------------+
|       Aplicacions           |
+-----------------------------+
|    Android Framework        |
+-----------------------------+
| Llibreries + Android Runtime|
+-----------------------------+
|            HAL              |
+-----------------------------+
|        Linux Kernel         |
+-----------------------------+
```

## Linux Kernel

És la base del sistema i s'encarrega, entre altres funcions, de:

- processos;
- memòria;
- xarxa;
- controladors;
- gestió del hardware;
- mecanismes de seguretat.

> Els apunts originals fan referència al Linux 2.6. Aquesta és una referència històrica; les versions modernes d'Android utilitzen versions molt posteriors del kernel.

## HAL

HAL significa **Hardware Abstraction Layer**.

Proporciona una abstracció entre el hardware i les capes superiors.

## Llibreries i Android Runtime

Android disposa de llibreries natives i d'Android Runtime (ART), que proporciona l'entorn d'execució de les aplicacions.

## Android Framework

Ofereix APIs i serveis per a les aplicacions, com ara:

- activitats;
- notificacions;
- finestres;
- recursos;
- localització;
- sensors;
- gestió de paquets.

## Capa d'aplicacions

És la capa on s'executen les aplicacions del sistema i les aplicacions instal·lades per l'usuari.
