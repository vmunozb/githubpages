<!--
  <<< Author notes: Header of the course >>>
  Include a 1280×640 image, course title in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Add your open source license, GitHub uses Creative Commons Attribution 4.0 International.
-->

# GitHub Pages

_Crea un sitio o un blog a partir de tus repositorios de GitHub con GitHub Pages._

<!--
  <<< Author notes: Start of the course >>>
  Include start button, a note about Actions minutes,
  and tell the learner why they should take the course.
  Each step should be wrapped in <details>/<summary>, with an `id` set.
  The start <details> should have `open` as well.
  Do not use quotes on the <details> tag attributes.
-->

<!--step0

Con GitHub Pages, puedes alojar blogs de proyectos, documentación, currículos, portafolios o cualquier otro contenido estático que desees. Tu repositorio de GitHub puede convertirse fácilmente en su propio sitio web. En este curso, te mostraremos cómo configurar tu propio sitio o blog utilizando GitHub Pages.

- **A quién va dirigido**: Principiantes, estudiantes, gestores de proyectos, pequeñas empresas.
- **Qué aprenderás**: Cómo construir un sitio web usando GitHub Pages.
- **Qué construirás**: Construiremos un sitio simple de GitHub Pages con un blog. Usaremos [Jekyll](https://jekyllrb.com), un generador de sitios estáticos.
- **Requisitos**: Si necesitas aprender sobre ramas, commits y pull requests, toma primero [Introducción a GitHub](https://github.com/DeustoKom/introduccion-a-github). Para saber más acerca de cómo formatear tu contenido usando Markdown, sigue [Comunicar usando Markdown](https://github.com/DeustoKom/comunicar-usando-markdown).
- **Cuánto tiempo**: Este curso consta de cinco pasos y tardarás menos de una hora en completarlo.

## Cómo empezar este curso

1. Encima de estas instrucciones, haz clic con el botón derecho del ratón en **Use this template** y abre el enlace en una nueva pestaña.<br />
   ![Use this template](https://user-images.githubusercontent.com/1221423/169618716-fb17528d-f332-4fc5-a11a-eaa23562665e.png)
2. En la nueva pestaña, sigue las indicaciones para crear un nuevo repositorio.
   - En **Owner**, elije tu cuenta personal para alojar el repositorio.
   - Recomendamos crear un repositorio público - los repositorios privados [utilizarán minutos de Acciones](https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions).
   ![Create a new repository](https://user-images.githubusercontent.com/1221423/169618722-406dc508-add4-4074-83f0-c7a7ad87f6f3.png)
3. Una vez creado tu nuevo repositorio, espera unos 20 segundos y actualiza la página. Sigue las instrucciones paso a paso en el README del nuevo repositorio.

endstep0-->

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

<details id=1>
<summary><h2>Paso 1: Habilita GitHub Pages</h2></summary>

_¡Bienvenida/o a GitHub Pages y Jekyll :tada:!_

El primer paso es habilitar GitHub Pages en este [repositorio](https://docs.github.com/en/get-started/quickstart/github-glossary#repository). Cuando habilitas GitHub Pages en un repositorio, GitHub toma el contenido que está en la rama principal `main` y publica una página web basada en su contenido.

### :keyboard: Actividad: Habilita GitHub Pages

1. Abre una nueva pestaña del navegador, y trabaja en los pasos de tu segunda pestaña mientras lees las instrucciones en esta pestaña.
1. Debajo del nombre de tu repositorio, haga clic en **Settings**.
1. Haz clic en **Pages**, en la sección "GitHub Pages", utiliza el desplegable **Source**, y luego selecciona **main branch**.
1. Espera alrededor de _un minuto_, luego actualiza esta página para el siguiente paso.
   > Al activar GitHub Pages se crea un despliegue (o _deploy_) de tu repositorio. Las acciones de GitHub pueden tardar hasta un minuto en responder mientras se espera el despliegue. Los próximos pasos serán de unos 20 segundos; este primer paso es más lento.

</details>

<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  Historic note: previous version checked for empty pull request, changed to the correct theme `minima`.
-->

<details id=2>
<summary><h2>Paso 2: Configura tu sitio</h2></summary>

_¡Has habilitado GitHub Pages!_ :tada:

Trabajaremos en una rama, `my-pages`, que hemos creado para ti para que este sitio se vea bien. :sparkle:

Jekyll utiliza un archivo titulado `_config.yml` para almacenar la configuración de tu sitio, tu tema, y el contenido reutilizable como el título de tu sitio y la dirección de GitHub. Puedes consultar el archivo `_config.yml` en la pestaña **Code** de tu repositorio.

Tenemos que utilizar un tema preparado para blogs. Para esta actividad, utilizaremos un tema llamado "minima".

### :keyboard: Actividad: Configura tu sitio

1. Busca el archivo `_config.yml` en la rama `my-pages`.
1. En la esquina superior derecha, abre el editor de archivos.
1. Añade un `theme:` establecido en **minima** para que aparezca en el archivo `_config.yml` como se indica a continuación:
    ```yml
    theme: minima
    ```
1. (Opcional) Puedes modificar las otras variables de configuración como `title:`, `author:`, y `description:` para personalizar aún más tu sitio.
1. Confirma los cambios.
1. Espera unos 20 segundos y actualiza esta página para el siguiente paso.

</details>

<!--
  <<< Author notes: Step 3 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  Historic note: previous version checked the homepage content was not empty.
-->

<details id=3 open>
<summary><h2>Paso 3: Personaliza tu página de inicio</h2></summary>

_¡Buen trabajo estableciendo el tema! :sparkles:_

Puedes personalizar tu página de inicio añadiendo contenido a un archivo `index.md` o al archivo `README.md`. GitHub Pages busca primero un archivo `index.md`. Tu repositorio tiene un archivo `index.md`, por lo que podemos actualizarlo para incluir tu contenido personalizado.

### :keyboard: Actividad: Crea tu página de inicio

1. Busca el archivo `index.md` en la rama `my-pages`.
1. En la esquina superior derecha, abre el editor de archivos.
1. Escribe el contenido que deseas mostrar en tu página de inicio. Puedes utilizar el formato Markdown en esta página.
1. (Opcional) También puedes modificar `title:` o simplemente ignorarlo por ahora. Lo discutiremos en el siguiente paso.
1. Confirma tus cambios en la rama `my-pages`.
1. Espera unos 20 segundos y actualiza esta página para el siguiente paso.

</details>

<!--
  <<< Author notes: Step 4 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  Historic note: previous version checked the file path. Previous version checked the front matter formatting.
-->

<details id=4>
<summary><h2>Paso 4: Crea un post en el blog</h2></summary>

_¡Tu página de inicio se ve genial! :cowboy_hat_face:_

GitHub Pages utiliza Jekyll. En Jekyll, podemos crear un blog utilizando archivos con nombres específicos y _frontmatter_ o cabeceras de archivo. Los archivos deben llamarse `_posts/AAAA-MM-DD-title.md`. También debes incluir `title` y `date` en tu _frontmatter_.

**¿Qué es el _frontmatter_?** La sintaxis que usan los archivos Jekyll se llama YAML frontmatter. Va en la parte superior de su archivo y se parece a esto:


```yml
---
title: "Bienvenida/o a mi blog"
date: 2022-11-03
---
```

Para más información sobre la configuración del _frontmatter_, consulta la [documentación de _frontmatter_ en Jekyll](https://jekyllrb.com/docs/frontmatter/).

### :keyboard: Actividad: Crea un post

1. Navega hasta la rama `my-pages`.
1. Haz clic en el menú desplegable `Add file` y luego en `Create new file`.
1. Nombra el archivo `_posts/AAAA-MM-DD-title.md`.
1. Sustituye el `AAAA-MM-DD` por la fecha de hoy, y cambia el `title` de tu primera entrada del blog si lo deseas.
   > Si editas el título, asegúrate de que hay guiones entre las palabras.
   > Si la fecha de la entrada de tu blog no sigue la convención de fechas correcta, recibirás un error y tu sitio no se construirá. Para obtener más información, consulta "[Error en la creación de la página: fecha de publicación no válida](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/troubleshooting-jekyll-build-errors-for-github-pages-sites)".
1. Escribe el siguiente contenido en la parte superior de la entrada de tu blog:
   ```yaml
   ---
   title: "TU TÍTULO"
   date: AAAA-MM-DD
   ---
   ```
1. Sustituye "TU TÍTULO" por el título de tu entrada en el blog.
1. Sustituye "AAAA-MM-DD" por la fecha de hoy.
1. Escribe un borrador rápido de tu entrada en el blog. Recuerda que siempre puedes editarlo más tarde.
1. Confirma los cambios en tu rama.
1. Espera unos 20 segundos y actualiza esta página para el siguiente paso.

</details>

<!--
  <<< Author notes: Step 5 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

<details id=5>
<summary><h2>Paso 5: Fusiona tu pull request</h2></summary>

_¡Buen trabajo :heart:! Todo el mundo podrá leer tu blog en un momento..._

Ahora puedes [fusionar](https://docs.github.com/en/get-started/quickstart/github-glossary#merge) tu pull request.

### :keyboard: Actividad: Fusiona tu pull request

1. Haz clic en **Merge pull request**.
1. Elimina la rama `my-pages` (opcional).
1. Espera unos 20 segundos y actualiza esta página para el siguiente paso.

</details>

<!--
  <<< Author notes: Finish >>>
  Review what we learned, ask for feedback, provide next steps.
-->

<details id=X>
<summary><h2>Finalización</h2></summary>

_¡Enhorabuena, has completado el curso!_

<img src=https://octodex.github.com/images/constructocat2.jpg alt=celebrate width=300 align=right>

¡Tu blog ahora está visible y se ha desplegado!

Aquí tienes un resumen de todas las tareas que has realizado en tu repositorio:

- Has habilitado GitHub Pages.
- Has seleccionado un tema usando el archivo de configuración.
- Has aprendido sobre el formato de directorio y las convenciones de nomenclatura de archivos en Jekyll.
- Has creado tu primera entrada de blog con Jekyll.

### ¿Y ahora, qué?

- Sigue trabajando en tu sitio de GitHub Pages... ¡nos encanta ver lo que se te ocurre!
- Nos encantaría saber qué te ha parecido este curso [en nuestro foro de debate](https://github.com/skills/.github/discussions).
- [Haz otro curso de GitHub Skills](https://github.com/skills).
- Lee los documentos de inicio de GitHub](https://docs.github.com/en/get-started).
- Para encontrar proyectos a los que contribuir, consulta [GitHub Explore](https://github.com/explore).

</details>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/skills/.github/discussions) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2022 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [CC-BY-4.0 License](https://creativecommons.org/licenses/by/4.0/legalcode)
