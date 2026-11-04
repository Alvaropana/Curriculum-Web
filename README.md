# Currículum web: Álvaro Peña Gil

Página web de mi currículum, hecha con [Astro](https://astro.build). Toda la información (datos personales, formación, experiencia, proyectos y contacto) está guardada en un archivo JSON y se pinta con componentes.

## Diseño

Este es mi diseño del Figma: https://www.figma.com/design/TvpghDRBsi6sZ0qHpB1iPX/Mi-curriculum?node-id=0-1&t=MEgmV82mrD59GdHM-1

Dentro del proyecto también está el documento Word del diseño: diseño pagina web curriculum

## Estructura del proyecto

```text
/
├── public/
    ├── foto perfil.jpg
    ├── foto de base de datos.png
    ├── image gmail.png
    ├── image monroy.png
    ├── image vedruna.png
    ├── imgane dirrecion.png
    ├── imagen telefono.png
    ├── logo nombre.png
    ├── Menu.png
│   └── 
├── src/
│   ├── components/
│   │   ├── CardExperiencia.astro
│   │   ├── CardFormacion.astro
│   │   ├── CardProyecto.astro
│   │   ├── Footer.astro
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   └── Titulo.astro
│   ├── data/
│   │   └── curriculum.json
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

## Cómo funciona

- `src/data/curriculum.json` guarda todo el contenido del currículum.
- `src/pages/index.astro` lee el JSON y, con `.map()`, crea una tarjeta por cada estudio, trabajo y proyecto.
- Cada parte de la página es un componente que recibe sus datos por props.
- Los colores y la fuente se definen una sola vez en `Layout.astro`, como variables CSS.

Para añadir un trabajo, un estudio o un proyecto nuevo basta con añadir un objeto al JSON, sin tocar los componentes.

## Comandos

Todos los comandos se ejecutan desde la raíz del proyecto, en una terminal:

| Comando           | Acción                                              |
| :---------------- | :-------------------------------------------------- |
| `npm install`     | Instala las dependencias                            |
| `npm run dev`     | Inicia el servidor local en `localhost:4321`        |

## Tecnologías

- Astro
- HTML y CSS
- JSON para los datos
