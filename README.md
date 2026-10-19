# Memories-descargas

Repositorio **solo para las descargas** de Memories: aquí no hay código (el código está en el repo privado `Memories`).

GitHub Actions de `Memories` sube aquí, en **Releases**, cada versión compilada:

- `v0.N`: la APK de Android de cada compilación.
- `v1.0.N`: la app de ordenador (Mac y Windows).
- `ultima`: los archivos fijos que leen las apps para **actualizarse solas**
  (`version.json`, `escritorio-<plataforma>.json`) y los enlaces fijos para
  descargar e invitar (`Memories.apk`, `Memories-Mac.dmg`, `Memories-Windows.msi`;
  `memoriessync.vercel.app/descargar`, `/mac` y `/windows` apuntan aquí).

**Tiene que ser público.** Las apps descargan sin cuenta de GitHub: si el
repositorio es privado, GitHub responde «404» y en el móvil sale
«No se pudo comprobar (error 404)» al buscar actualizaciones (y fallan los
enlaces de descarga).
