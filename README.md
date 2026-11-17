# IA-27 - Descargas oficiales

Asistente virtual de escritorio **100 % local** de **Estalingrado Corp**.

- Ejecuta los modelos GGUF en la computadora del usuario: **sin cuentas, sin claves de API, sin servidores y sin conexión**.
- **Atenea Mini Beta** (2 B) viene incluido en el instalador.

## Descargas - v1.4.4

| Archivo | Descripción |
|---|---|
| [`IA-27-Setup-1.4.4.exe`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.4/IA-27-Setup-1.4.4.exe) | Instalador para Windows (x64). |
| [`IA-27-portable.exe`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.4/IA-27-portable.exe) | Versión portable: corre sin instalar. |
| [`IA-27-Setup-1.4.4.exe.blockmap`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.4/IA-27-Setup-1.4.4.exe.blockmap) | Datos de actualización automática. |

### Novedades de v1.4.4

- **El navegador deja de ser una caja negra.** Cuatro redes de seguridad nuevas:
  - **Techo de espera por acción.** Si una página se cuelga, el turno ya no queda "pensando" para siempre: el modelo recibe un mensaje que dice qué pasó y qué puede hacer.
  - **El texto de la página es evidencia no confiable.** Llega marcado como contenido externo: una web que intente darle instrucciones al modelo no puede pasar por órdenes del operador.
  - **Permisos acotados.** El Chromium del agente tiene una lista blanca mínima: cámara, micrófono, geolocalización, notificaciones y lectura del portapapeles quedan denegados.
  - **Panel automático sin robar el foco.** Cuando el modelo navega o interactúa, el panel del navegador se abre para que el operador vea lo que pasa. Se apaga en Ajustes, y si el operador lo cierra, no se vuelve a abrir solo.
- Sigue todo lo de la v1.4.3: las 5 primitivas de interacción con la página (clic, escribir, esperar, desplazarse, extraer), el modelo eligiendo el elemento por **índice**, confirmación antes de escribir o de hacer clic irreversible, y nunca escribiendo contraseñas.

### SHA256

```
IA-27-Setup-1.4.4.exe
  b7dcb4345b76ac99d50fb8ef956ae44255604748c4aa4a53f8821da4fd9057d2

IA-27-portable.exe
  517c6529143e166d5a806d6a4dacc4317db6c72e87089a8b3bc159b434279a06
```

## Requisitos

- Windows 10/11 (x64).
- El modelo incluido no requiere descarga adicional.

Más información: <https://estalingradocorp.com.ar>

---

© Estalingrado Corp
