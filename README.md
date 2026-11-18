# IA-27 - Descargas oficiales

Asistente virtual de escritorio **100 % local** de **Estalingrado Corp**.

- Ejecuta los modelos GGUF en la computadora del usuario: **sin cuentas, sin claves de API, sin servidores y sin conexión**.
- **Atenea Mini Beta** (2 B) viene incluido en el instalador.

## Descargas - v1.4.5

| Archivo | Descripción |
|---|---|
| [`IA-27-Setup-1.4.5.exe`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.5/IA-27-Setup-1.4.5.exe) | Instalador para Windows (x64). |
| [`IA-27-portable.exe`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.5/IA-27-portable.exe) | Versión portable: corre sin instalar. |
| [`IA-27-Setup-1.4.5.exe.blockmap`](https://github.com/nicotips27/IA27-downloads/releases/download/v1.4.5/IA-27-Setup-1.4.5.exe.blockmap) | Datos de actualización automática. |

### Novedades de v1.4.5

- **Se arregla el error que mataba las respuestas web.** Si le pedías algo que el
  router clasificaba como búsqueda o trabajo web (por ejemplo "buscá en la web el
  precio del dólar"), la app respondía `⚠ Assignment to constant variable.` y el
  modelo no contestaba nada. No era un problema del modelo: era un error de
  JavaScript en el motor que moría antes de generar.
  - **Por qué pasaba:** el presupuesto de herramientas se declaraba como
    constante y en la línea siguiente se "ajustaba" a 4 en el dominio web. Una
    constante no se puede reasignar, así que el turno moría en el acto. Solo
    pasaba en el dominio web y sin carpeta de trabajo activa, por eso pasó
    desapercibido. Venía de la v1.4.3 y afectaba también a la v1.4.4.
  - **Qué cambió:** el presupuesto se calcula de una sola vez (4 llamadas en el
    dominio web, 2 fuera de él, 8 con carpeta de trabajo) y ya no se toca
    después. Se agregó una prueba de regresión y un verificador
    (`npm run check:const`) que detecta cualquier reasignación de una constante.
- Sigue todo lo de la v1.4.4: el navegador Chromium integrado deja de ser una
  caja negra (techo de espera por acción, evidencia externa no confiable,
  permisos acotados y panel automático sin robar el foco), las 5 primitivas de
  interacción con la página (clic, escribir, desplazar, esperar y extraer), el
  modelo eligiendo el elemento por **índice**, confirmación antes de escribir o
  de hacer clic irreversible, y nunca escribiendo contraseñas.

### SHA256

```
IA-27-Setup-1.4.5.exe
3f63bb0940b37d644603d223d2d070b83bca7fa00d3eb228b4f2e44996a9b878

IA-27-portable.exe
49b02bbfd1cf09cb53de654d39ef49237fac9414461cc712745e3cebb455f1ae
```

## Requisitos

- Windows 10/11 (x64).
- El modelo incluido no requiere descarga adicional.

Más información: <https://estalingradocorp.com.ar>

---

© Estalingrado Corp
