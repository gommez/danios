# DANI OS

Sistema operativo doméstico personal. App web estática, sin backend, sin frameworks.

## Características

- Entrada universal por texto y voz (Web Speech API)
- Clasificador automático de módulos: Compra, Mascotas, Gastos, Limpieza, Citas, Hogar
- Motor de imputación de gastos con subcategorías (Alimentación, Restauración, Ocio, Hogar, Transporte, Salud…)
- Confirmación conversacional por voz
- Contextos NFC — etiquetas imantadas por zona del hogar
- Dashboard con pulso doméstico en tiempo real
- Persistencia en localStorage
- Tema claro / oscuro con un toque
- Exportar / importar JSON
- Funciona offline, sin servidor

## Archivos

```
index.html   — app completa (HTML + CSS + JS embebidos)
README.md    — este archivo
```

## Uso

Abre `index.html` en el navegador. No necesita servidor.

Para GitHub Pages: activa Pages desde la rama `main`, directorio raíz.  
URL resultante: `https://[usuario].github.io/[repo]/`

## NFC

En Ajustes (⚙) → sección NFC → copia la URL de cada zona y grábala en la etiqueta.

Contextos disponibles: Zona Mascotas · Cocina · Limpieza · Coche · Gastos · Escritorio

## Casos de uso probados

| Entrada | Módulo | Categoría |
|---|---|---|
| `Tomates` | COMPRA | — |
| `Tomates 5€` | GASTOS | Alimentación |
| `Orlando 5,65€` | GASTOS | Restauración |
| `IKEA 120€` | GASTOS | Hogar |
| `Amazon 28€` | GASTOS | General (pide imputación) |
| `+50 bizum recibido` | GASTOS | Ingresos |
| `Verdita comió` | MASCOTAS | — |
| `Cita médico lunes` | CITAS | — |
| `Limpiar baño` | LIMPIEZA | — |

## Versión

v0.6 — Mayo 2025
