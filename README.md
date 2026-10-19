# Memories-descargas

Repositorio **solo para las descargas** de Memories: aquí no hay código (el código está en el repo privado `Memories`).

GitHub Actions de `Memories` sube aquí, en **Releases**, cada versión compilada:

- `v0.N`: la APK de Android de cada compilación.
- `v1.0.N`: la app de ordenador (Mac y Windows).
- `ultima`: los archivos fijos que leen las apps para **actualizarse solas**
  (`version.json`, `escritorio-<plataforma>.json`) y los enlaces fijos para
  descargar e invitar (`Memories.apk`, `Memories-Mac.dmg`, `Memories-Windows.msi`;
  `memoriessync.vercel.app/descargar`, `/mac` y `/windows` apuntan aquí).

**Puede ser privado.** Las apps no descargan de aquí directamente sino por
`memoriessync.vercel.app/d/<versión>/<archivo>`, que entra en GitHub con el token
`DESCARGAS_TOKEN` (variable de entorno del proyecto de Vercel, con permiso
*Contents: Read-only* sobre este repositorio). Si esa variable no está puesta,
el servidor manda al enlace público de GitHub y entonces el repositorio sí
tiene que ser público (si no, sale «error 404» al buscar actualizaciones).
