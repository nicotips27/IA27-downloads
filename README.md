# IA-27 - Descargas oficiales

Asistente virtual de escritorio **100 % local** de **Estalingrado Corp**.

- Ejecuta los modelos GGUF en la computadora del usuario: **sin cuentas, sin claves de API, sin servidores y sin conexión**.
- **Atenea Mini Beta** (2 B) viene incluido en el instalador.

## Descargas - v1.4.3

| Archivo | Descripción |
|---|---|
| [`IA-27-Setup-1.4.3.exe`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.3/IA-27-Setup-1.4.3.exe) | Instalador para Windows (x64). |
| [`IA-27-portable.exe`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.3/IA-27-portable.exe) | Versión portable: corre sin instalar. |
| [`IA-27-Setup-1.4.3.exe.blockmap`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.3/IA-27-Setup-1.4.3.exe.blockmap) | Datos de actualización automática. |

### Novedades de v1.4.3

- **El modelo ya interactúa con la página, no solo la lee.** El navegador Chromium integrado suma 5 primitivas: hacer clic, escribir en un campo, esperar a que aparezca un elemento, desplazarse y extraer el texto de un elemento puntual (el precio de un producto, la celda de una tabla). El modelo elige el elemento por **índice** (el número que vio en la lista de elementos interactivos), no por selectores inventados.
- **Seguro por diseño:** escribir siempre pide confirmación y nunca completa contraseñas; hacer clic pide confirmación solo si la acción es irreversible (borrar, comprar, publicar, pagar…); el panel del navegador muestra la misma vista que el modelo.
- Sigue todo lo de la v1.4.2: el navegador Chromium integrado como modo web por defecto, modo API sin silencio con **Probar conexión** e **iconos SVG de Lucide** en botones y chips de herramientas.

### SHA256

```
IA-27-Setup-1.4.3.exe
  4300efafb035551ce834fe9ee825debe0e4f4aa25cd706f65e66aedc64bdbf78

IA-27-portable.exe
  6c705c8fec55367ac70badf99c6f9a2e55c0e595da5a345ec38b494521aa2aab
```

## Requisitos

- Windows 10/11 (x64).
- El modelo incluido no requiere descarga adicional.

Más información: <https://estalingradocorp.com.ar>

---

© Estalingrado Corp
