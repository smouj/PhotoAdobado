# PhotoAdobado — procedencia y cambios

## Origen

- Upstream: https://github.com/storytold/photocraft
- Commit base: 03d0c7e3b39cfb401cdbba590431141ee4c6c8fa (2026-10-19)
- Licencia del código: MIT OR Apache-2.0
- Copyright original: ArtCraft Team and the PhotoCraft contributors.

## Cambios de esta distribución

- Nombre de producto visible: PhotoAdobado (el crate y el ejecutable internos siguen siendo photocraft para no romper el workspace).
- Título de ventana, nombre de aplicación y textos de About.
- Enlaces de ayuda, GitHub e issues apuntando a smouj/PhotoAdobado y a Adobado Kit.
- Iconos de aplicación sustituidos por la identidad de PhotoAdobado.
- README propio. Se retiran los logos y assets de marca de ArtCraft.
- No se han cambiado el motor de imagen, los formatos ni las funciones de edición.

## Estado de validación — 20/10/2026

- **Build de Windows:** correcto en GitHub Actions ([workflow](https://github.com/smouj/PhotoAdobado/actions/workflows/windows-build.yml)).
- **Prueba manual:** app instalada y abierta en Windows.
- **Uso con archivos reales:** abrir, modificar y exportar sigue pendiente.
- **Distribución:** hay una release alpha anterior al icono actual; su ZIP conserva el icono previo y debe actualizarse después de probar el nuevo binario.
- **Origen:** 03d0c7e3b39cfb401cdbba590431141ee4c6c8fa.

## Marcas

ArtCraft, PhotoCraft y sus logos son marcas del ArtCraft Team y no están cubiertos por la licencia de código. Esta distribución no los usa. Adobe y Photoshop son marcas de Adobe Inc.; este proyecto no está afiliado a Adobe.

## Aviso

Esta es una distribución modificada. Las modificaciones son de @smouj (2026). El código original conserva sus avisos de copyright y licencia.
