# Sistema de Gestión SeCyT - Prototipo Web

Plataforma web institucional desarrollada para la Secretaría de Ciencia y Tecnología (SeCyT) de la Universidad Tecnológica Nacional, Facultad Regional San Francisco. Este proyecto nace como trabajo práctico para la cátedra de Análisis de Sistemas de Información.

## Objetivo del Proyecto

El sistema busca resolver la fragmentación de la información y la alta carga operativa del área de gestión. Reemplaza el uso de múltiples planillas Excel descentralizadas por un sistema unificado que permite:
* Gestionar currículums y perfiles de investigadores de forma centralizada.
* Hacer un seguimiento ágil de proyectos (PID).
* Generar reportes.

## Tecnologías Utilizadas

* **Runtime / Package Manager:** [Bun](https://bun.sh/)
* **Framework:** [Astro](https://astro.build/)
* **Estilos:** CSS puro aplicando metodología **BEM** (Block, Element, Modifier).
* **Datos (Prototipado):** Archivos `.csv` locales.

## Modelo de Dominio (MVP)

El sistema central se apoya en cuatro entidades fundamentales para resolver la interoperabilidad de los datos:
* **UsuarioGestion:** Personal administrativo y directivo (Secretaría) con permisos de auditoría, edición y exportación de reportes.
* **Investigador:** Docentes, alumnos y graduados. Cuentan con permisos mínimos enfocados en la actualización de su CV y visualización de historial.
* **Proyecto:** Iniciativas de investigación con estado asignado.
* **Participacion:** Resuelve la relación de muchos a muchos, registrando el rol específico y la dedicación de cada investigador dentro de un proyecto.

## Instalación y Ejecución Local

Para correr este prototipo en tu máquina local, sigue estos pasos:

1. **Clonar el repositorio:**
```bash
git clone [https://github.com/anladner-clone/Prototipo-SECyT-v2.git](https://github.com/anladner-clone/Prototipo-SECyT-v2.git)
```
2. **Instalar dependencias:**
```bash
cd Prototipo-SECyT-v2
bun install
```

3. **Levantar el servidor de desarrollo:**
```bash
bun run dev
```


El prototipo estará disponible en `http://localhost:4321`.

## Equipo de Desarrollo

* Ariel Ladner
* Julio Arrieta
* Ivan Naz
* Franco Fraga
