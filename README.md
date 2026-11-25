# LaneLoader

Reproductor web que carga niveles de Sonolus desde un servidor o desde un archivo `.scp`,
envuelto en una app para iPad con iOS 12 (probado en la idea, no en hardware real).

## Obtener el IPA
1. Sube este repositorio a GitHub.
2. Pestaña **Actions → Build IPA → Run workflow**.
3. Descarga el artefacto `LaneLoader-ipa`.

El IPA sale **sin firmar**. Para instalarlo hay que firmarlo con tu Apple ID
(Sideloadly o AltStore). Comprueba que la versión de la herramienta soporte iOS 12.

## Pasar niveles del iPhone/PC al iPad
En Sonolus: abre tu colección, pulsa **Export** y guarda el `.scp`.
Llévalo al iPad (AirDrop, iCloud Drive, correo) y, en la app, pulsa **Importar .scp**.
Si el `.scp` es de otra versión de Sonolus (0.5.13 vs 0.6.0), existe el convertidor
`sevenc-nanashi/scp-converter`.

## Estado
Carga y descomprime nivel + motor. Falta el intérprete de nodos, el render y el audio.
