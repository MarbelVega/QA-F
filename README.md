# Quality Engineering Framework

Sitio estático para GitHub Pages con **120 escenarios de prueba**, buscador, filtros y referencias a estándares.

## Publicar en GitHub Pages

1. Crea un repositorio y carga todo el contenido de este ZIP en la raíz.
2. En **Settings > Pages**, selecciona **GitHub Actions**.
3. Haz push a `main`. El workflow desplegará el sitio.

## Desarrollo local

```bash
python -m http.server 8000
```

Abre `http://localhost:8000`.

## Alcance

Web/Frontend, API, Backend, Base de datos, Mobile, Performance, Seguridad, Accesibilidad, Datos/IA, Infraestructura/Cloud, Desktop, IoT y prácticas transversales.

## Estructura

- `index.html`: portal
- `data/scenarios.json`: catálogo editable
- `data/standards.json`: referencias
- `docs/strategy.md`: estrategia y gobierno
- `.github/workflows/pages.yml`: despliegue automático
- `CONTRIBUTING.md`: guía de contribución

## Uso responsable

Las pruebas de seguridad deben ejecutarse únicamente sobre activos autorizados, con alcance, ventana, responsables y plan de contingencia definidos.
