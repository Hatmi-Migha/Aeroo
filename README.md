# Aerolab Center · Plataforma interactiva para aprender Python

Versión visual V2.3 construida sobre la lógica educativa de AeroPy V2.2.

La interfaz principal fue rediseñada para seguir el segundo concepto aprobado: identidad visible de **Aerolab Center Creative Minds**, navegación lateral, buscador superior, portada a pantalla completa, la imagen seleccionada por el proyecto en lugar del robot y panel de progreso integrado.

## Qué incluye

### Contenido educativo

- 60 misiones principales: 20 Explorador, 20 Creador y 20 Developer.
- 12 retos especiales.
- 6 mini-proyectos.
- 3 proyectos finales.
- 81 actividades evaluables.
- 3 bloques por nivel con Jefes de bloque.
- Laboratorio Python para proyectos libres.

### Aprendizaje adaptativo

- Prueba inicial de 8 preguntas para recomendar el punto de inicio.
- Recomendaciones según intentos fallidos, pistas utilizadas y ritmo de avance.
- “Revisión de vuelo” automática cada 5 misiones.
- Ruta progresiva Explorador → Creador → Developer.

### Ayudas dentro de los ejercicios

- Tres niveles de pistas.
- “¿Qué hace esta línea?”.
- Ejecución paso a paso con visualización de variables.
- Mensajes de error simplificados.
- Diccionario Python integrado.
- Historial local de intentos.
- Resumen de conceptos al resolver un ejercicio.
- Desafíos creativos opcionales.

## Diseño V2.3

- Logotipo de Aerolab Center en la navegación principal.
- Sidebar: Inicio, Ruta, Misiones, Laboratorio, Progreso, Logros y Configuración.
- Buscador de lecciones y temas.
- Hero oscuro/azul inspirado en el segundo mockup aprobado.
- Imagen indicada por el proyecto reemplazando a la mascota robot.
- Panel de XP, estrellas, misiones y progreso integrado.
- Botones naranja y azul coherentes con la identidad visual.
- Sin footer visible con la marca AeroPy.
- Diseño responsive para computadora, tablet y móvil.

## Ejecutar

```bash
npm install
npm run dev
```

Vite mostrará una dirección local, normalmente:

```text
http://localhost:5173/
```

## Compilar para producción

```bash
npm run build
```

`vite.config.js` utiliza `base: './'`, por lo que el build queda preparado para alojarse en una subcarpeta o en GitHub Pages.

## Consideraciones

Pyodide se carga desde CDN la primera vez que se ejecuta Python. El progreso, preferencias e intentos se almacenan localmente y no requieren cuenta.

## Archivos visuales principales

- `public/brand/aerolab-logo.png`
- `public/hero/python-character.jpg`
- `src/components/Header.jsx`
- `src/pages/HomePage.jsx`
- `src/index.css`

## Archivos educativos principales

- `src/data/course.js`
- `src/data/placement.js`
- `src/data/glossary.js`
- `src/utils/learningEngine.js`
- `src/pages/LessonPage.jsx`
- `src/components/StepVisualizer.jsx`
- `src/workers/pythonWorker.js`
