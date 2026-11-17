# IA-27 - Descargas oficiales

Asistente virtual de escritorio **100 % local** de **Estalingrado Corp**.

- Ejecuta los modelos GGUF en la computadora del usuario: **sin cuentas, sin claves de API, sin servidores y sin conexión**.
- **Atenea Mini Beta** (2 B) viene incluido en el instalador.

## Descargas - v1.4.2

| Archivo | Descripción |
|---|---|
| [`IA-27-Setup-1.4.2.exe`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.2/IA-27-Setup-1.4.2.exe) | Instalador para Windows (x64). |
| [`IA-27-portable.exe`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.2/IA-27-portable.exe) | Versión portable: corre sin instalar. |
| [`IA-27-Setup-1.4.2.exe.blockmap`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.2/IA-27-Setup-1.4.2.exe.blockmap) | Datos de actualización automática. |

### Novedades de v1.4.2

- **El navegador Chromium integrado pasa a ser el modo web por defecto del modelo.** Antes, para leer una página el modelo necesitaba dos tool-calls (abrir y leer) y el presupuesto por mensaje es de dos: el prefetch de búsqueda se llevaba uno y la lectura se quedaba sin ejecutar. Ahora `navegador_navegar` abre la URL y devuelve el contenido renderizado en una sola llamada, el prefetch tiene presupuesto propio, la política del navegador viaja en el prompt y el Chromium queda disponible en todas las especialidades.
- Sigue todo lo de la v1.4.1: modo API sin silencio (razonamiento visible + **Probar conexión**) e **iconos SVG de Lucide** en botones y chips de herramientas.

### SHA256

```
IA-27-Setup-1.4.2.exe
  ea869301e6175654e5874ccfc9e44d8d883612412d9b6680f6f61b2147e1092b

IA-27-portable.exe
  476f7bd35804d7dbd4664faf5e8cb74ffc8fedf52277adc81d09525ddd16647c
```

## Requisitos

- Windows 10/11 (x64).
- El modelo incluido no requiere descarga adicional.

Más información: <https://estalingradocorp.com.ar>

---

© Estalingrado Corp
