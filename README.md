# PhotoAdobado

<p align="center"><img src="assets/adobado/icon.png" width="104" alt="PhotoAdobado"></p>

[![License](https://img.shields.io/badge/license-MIT%20OR%20Apache--2.0-6cb6ff)](LICENSE-MIT)
[![Rust](https://img.shields.io/badge/Rust-1.95%2B-ff7a59)](Cargo.toml)
[![Windows build](https://github.com/smouj/PhotoAdobado/actions/workflows/windows-build.yml/badge.svg?branch=main)](https://github.com/smouj/PhotoAdobado/actions/workflows/windows-build.yml)
[![Prueba](https://img.shields.io/badge/prueba-inicio%20comprobado-6cb6ff)](#estado)
[![Estrellas](https://img.shields.io/github/stars/smouj/PhotoAdobado?style=flat&color=B8F34A)](https://github.com/smouj/PhotoAdobado/stargazers)
[![Adobado Kit](https://img.shields.io/badge/Adobado%20Kit-hub-b8f34a)](https://github.com/smouj/Adobado_Kit)

Retoca imágenes con capas, máscaras, ajustes y compatibilidad declarada con PSD.

> **Pruebas en Windows (21/10/2026):** la compilación, la instalación y el inicio se han comprobado. Aún falta probar un flujo completo con un archivo real: abrirlo, editarlo y exportarlo.
>
> Proyecto independiente. No afiliado a ArtCraft ni a Adobe.

![PhotoAdobado — captura real de la aplicación](docs/screenshot.png)

<sub>Captura real de la aplicación en Windows.</sub>

## Estado

- **Build de Windows:** correcto en GitHub Actions; consulta el [workflow actual](https://github.com/smouj/PhotoAdobado/actions/workflows/windows-build.yml).
- **Instalación e inicio:** comprobados en Windows el 21/10/2026.
- **Prueba con un archivo:** aún falta completar el flujo de abrir, editar y exportar.
- **Estado:** alpha; aún falta validar un flujo completo con un archivo real.
- **Descarga pública:** [v0.1.0-alpha.1](https://github.com/smouj/PhotoAdobado/releases/tag/v0.1.0-alpha.1) es una versión alpha y conserva el icono anterior. El flujo con archivos reales aún no está validado; tenlo en cuenta antes de descargarla.
- **Commit de origen:** 03d0c7e3b39cfb401cdbba590431141ee4c6c8fa.

## Qué incluye

- Capas, máscaras, grupos y estilos de capa.
- Ajustes no destructivos, curvas, niveles y color.
- Texto, vectores, pinceles y selecciones.
- Lectura y escritura de PSD, además de formatos de imagen habituales.
- Interfaz nativa en Rust con egui/wgpu; sin Electron ni webview.
- Funciona sin conexión y sin cuentas.

Estas funciones corresponden al proyecto base. La compatibilidad declarada con PSD y otros formatos aún no se ha comprobado aquí mediante un flujo con archivos reales.

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

Hecho por @smouj.
