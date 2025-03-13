# Proyecto de Seguridad Informática

Este repositorio contiene un sitio web informativo sobre seguridad informática, desarrollado como proyecto para el Modulo 1. El sitio consta de 5 páginas HTML con información sobre diversos aspectos de la ciberseguridad.

## Estructura del Sitio

- **index.html**: Página principal con introducción a la seguridad informática
- **amenazas.html**: Información sobre amenazas comunes (malware, phishing, etc.)
- **proteccion.html**: Métodos y estrategias de protección
- **recursos.html**: Herramientas y recursos útiles
- **contacto.html**: Formulario de contacto e información

## Flujo de Trabajo Git

El proyecto fue desarrollado siguiendo un flujo de trabajo de ramas con:
- Rama principal: `main` 
- Rama de desarrollo: `develop`
- Ramas de características: `feature/nombre-pagina`

### Comandos utilizados para cada página

Para cada una de las 5 páginas, se siguió este proceso:

#### 1. Página principal (index.html)

```bash
git checkout develop
git checkout -b feature/index
# Crear/editar index.html
git add index.html
git commit -m "Creación de la página principal (index.html)"
git push -u origin feature/index
git checkout develop
git merge --no-ff feature/index -m "Merge: Integración de página principal"
git push origin develop

