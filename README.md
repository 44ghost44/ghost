# ghost

`ghost.sh` es una herramienta bash sencilla y visual que te ayuda a poner tu interfaz WiFi en modo monitor.

---

## ¿Qué hace este script?

- Busca tus interfaces WiFi disponibles.
- Te permite seleccionar la interfaz (si hay varias).
- Mata procesos que pueden interferir con el modo monitor.
- Cambia la interfaz al modo monitor en el canal que elijas.
- Informa si la interfaz está correctamente en modo monitor y en el canal seleccionado.

---

## Este script es útil para:

- Quienes necesitan poner una interfaz WiFi en modo monitor rápidamente.

---

## ¿Qué adaptadores WiFi soporta?

- Funciona con cualquier tarjeta/adaptador WiFi que soporte modo monitor y sea reconocida por `iw` y `iwconfig`.
- No todos los adaptadores USB soportan modo monitor. Verifica la compatibilidad de tu hardware :)

---

## Requisitos

- Bash
- utils: `iw`, `iwconfig`, `airmon-ng`, `ip`
- Permisos de sudo para cambiar el modo de la interfaz
- Terminal con soporte UTF-8 y ANSI colors (para ver bien el arte/firma)
- Adaptador WiFi compatible con modo monitor

---

## Uso

1. Da permisos de ejecución (solo la primera vez):

   ```bash
   chmod +x ghost.sh
   ```

2. Ejecuta el script:

   ```bash
   ./ghost.sh [canal]
   ```

   Si no indicas un canal, usará el canal 6 por defecto.

---

## Ejemplo de ejecución

```bash
./ghost.sh 11
```
Selecciona la interfaz y fija el canal 11 en modo monitor.

---

## Autor

Hecho por [44ghost44](https://github.com/44ghost44)

---
