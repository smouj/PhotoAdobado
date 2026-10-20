# PhotoAdobado

<p align="center"><img src="assets/adobado/icon.png" width="104" alt="PhotoAdobado"></p>

[![License](https://img.shields.io/badge/license-MIT%20OR%20Apache--2.0-6cb6ff)](LICENSE-MIT)
[![Rust](https://img.shields.io/badge/Rust-1.95%2B-ff7a59)](Cargo.toml)
[![Windows build](https://github.com/smouj/PhotoAdobado/actions/workflows/windows-build.yml/badge.svg?branch=main)](https://github.com/smouj/PhotoAdobado/actions/workflows/windows-build.yml)
[![Estado](https://img.shields.io/badge/status-Windows%20smoke%20test-6cb6ff)](#estado)
[![Estrellas](https://img.shields.io/github/stars/smouj/PhotoAdobado?style=flat&color=B8F34A)](https://github.com/smouj/PhotoAdobado/stargazers)
[![Adobado Kit](https://img.shields.io/badge/Adobado%20Kit-hub-b8f34a)](https://github.com/smouj/Adobado_Kit)

Editor de imagen nativo, local y open source. Derivado de PhotoCraft, rebrandeado para Adobado Kit.

> **Prueba de humo superada en Windows (20/10/2026).** Build de Windows correcta y app instalada y abierta en el PC. La prueba de abrir, modificar y exportar un archivo real sigue pendiente; el proyecto continúa en alpha.
>
> Proyecto independiente. No afiliado a ArtCraft ni a Adobe.

![PhotoAdobado — captura real de la aplicación](docs/screenshot.png)

<sub>Captura real de la aplicación en Windows.</sub>

## Estado

- **Build de Windows:** correcto en GitHub Actions; consulta el [workflow actual](https://github.com/smouj/PhotoAdobado/actions/workflows/windows-build.yml).
- **Prueba manual:** instalada y abierta en Windows el 20/10/2026.
- **Flujo funcional:** abrir, modificar y exportar un archivo real sigue pendiente.
- **Disponibilidad:** alpha; todavía no se declara lista para uso general.
- **Release pública:** [v0.1.0-alpha.1](https://github.com/smouj/PhotoAdobado/releases/tag/v0.1.0-alpha.1) se publicó antes de la identidad visual actual y conserva el icono anterior. El ZIP se actualizará después de verificar el icono integrado y la prueba funcional.
- **Commit de origen:** 03d0c7e3b39cfb401cdbba590431141ee4c6c8fa.

## Qué incluye

- Capas, máscaras, grupos y estilos de capa.
- Ajustes no destructivos, curvas, niveles y color.
- Texto, vectores, pinceles y selecciones.
- Lectura y escritura de PSD, además de formatos de imagen habituales.
- Interfaz nativa en Rust con egui/wgpu; sin Electron ni webview.
- Funciona sin conexión y sin cuentas.

La lista completa de funciones y su estado están en la documentación upstream. La madurez es la de PhotoCraft: alpha.

## Build

Requisitos: Rust 1.95 o superior.

    cargo run --release -p photocraft -- imagen.psd

En Windows, el binario sale en target/release/photocraft.exe. El nombre interno del crate y del ejecutable se conserva para no romper el workspace; el nombre de producto visible es PhotoAdobado.

## Procedencia y licencias

- Upstream: https://github.com/storytold/photocraft
- Commit base: 03d0c7e3b39cfb401cdbba590431141ee4c6c8fa
- Código: MIT OR Apache-2.0. Se conservan LICENSE-MIT, LICENSE-APACHE, NOTICE y ATTRIBUTION.md.
- Cambios de esta distribución: docs/ADOBADO.md.
- La marca, el wordmark y los logos de ArtCraft son trademarks y se han retirado de esta distribución.

## Adobado Kit

PhotoAdobado forma parte de Adobado Kit: https://github.com/smouj/Adobado_Kit

Hecho por SMOUJ013.
