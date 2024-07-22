# proyecto-colaborativo
Este proyecto es una prueba para el manejo de github
una vez que se haya clonado el repositorio, cada estudiante deberá seguir los siguientes pasos:

Modificar el archivo: `colaboradores.md`

Este archivo tendra la siguiente estructura:

1. Una lista de colaboradores
2. Una breve descripción del proyecto
3. Tareas pendientes
4. Citas favoritas de programación


5. Clonar el repositorio:
   ```
   git clone https://github.com/Dreycko/proyecto-colaborativo.git
   cd proyecto-colaborativo
   ```

6. Crear y cambiar a una nueva rama:
   ```
   git checkout -b modificacion-colaborador
   ```

7. Modificar el archivo `colaboradores.md`:
   Cada estudiante añadirá su nombre a la lista de colaboradores y realizará cambios en las otras secciones.

8. Commit y push de los cambios:
   ```
   git add colaboradores.md
   git commit -m "Añadido mi nombre y modificaciones"
   git push origin modificacion-colaborador
   ```

9. Crear un Pull Request en GitHub.
Entendido. Agregaré las imágenes utilizando código de markdown. Aquí tienes la sección actualizada:

 Crear Pull Requests:
   - Cada miembro va a GitHub, a la página del repositorio https://github.com/Dreycko/proyecto-colaborativo.
   
   - En el menú "Branch", selecciona la rama que contiene tus commits.
     
     ![Menú desplegable de ramas](https://docs.github.com/assets/cb-29825/mw-1440/images/help/pull_requests/branch-dropdown.webp)
     
     Esta imagen muestra el menú desplegable de ramas en la interfaz de GitHub, donde puedes seleccionar la rama específica que contiene tus cambios.

   - Sobre la lista de archivos, en el banner amarillo, haz clic en "Compare & pull request" para crear un Pull Request para la rama asociada.
     
     ![Botón Compare & pull request](https://docs.github.com/assets/cb-34097/mw-1440/images/help/pull_requests/pull-request-compare-pull-request.webp)
     
     Esta imagen muestra el banner amarillo con el botón "Compare & pull request" que aparece cuando una rama tiene cambios listos para ser propuestos como un Pull Request.

   - Usa el menú desplegable "base" para seleccionar la rama en la que deseas fusionar tus cambios (normalmente "main").
   - Usa el menú desplegable "compare" para elegir la rama temática en la que hiciste tus cambios.
   - Escribe un título y una descripción para tu Pull Request.
   - Para crear un Pull Request listo para revisión, haz clic en "Create Pull Request".
   - Para crear un borrador de Pull Request, usa el menú desplegable y selecciona "Create Draft Pull Request", luego haz clic en "Draft Pull Request".

Nota para los estudiantes: Las imágenes se mostrarán directamente en plataformas que soporten la visualización de markdown con imágenes. Si están viendo este tutorial en un formato de texto plano, pueden copiar los enlaces de las imágenes y pegarlos en su navegador para verlas.

1.  Para generar conflictos intencionalmente:
   - Dos o más estudiantes modificarán la misma línea o sección del archivo.
   - Por ejemplo, ambos podrían añadir una cita en la misma posición.

2.  Resolver conflictos:
   a. El estudiante que recibe el mensaje de conflicto al intentar hacer merge, ejecutará:
      ```
      git checkout main
      git pull origin main
      git checkout modificacion-colaborador
      git merge main
      ```
   
   b. Git marcará los conflictos en el archivo. Abrirlo en un editor y se verá algo así:
      ```
      <<<<<<< HEAD
      Cita añadida por el estudiante A
      =======
      Cita añadida por el estudiante B
      >>>>>>> main
      ```

   c. Editar el archivo para resolver el conflicto, decidiendo qué cambios mantener:
      ```
      Cita añadida por el estudiante A
      Cita añadida por el estudiante B
      ```

   d. Añadir el archivo modificado y hacer commit:
      ```
      git add colaboradores.md
      git commit -m "Resuelto conflicto en colaboradores.md"
      ```

   e. Pushear los cambios:
      ```
      git push origin modificacion-colaborador
      ```

3.  Actualizar el Pull Request en GitHub.

4.  Revisar y aprobar el Pull Request.

5.  Merge del Pull Request en la rama principal.

6.  Todos los estudiantes actualizan sus repositorios locales:
    ```
    git checkout main
    git pull origin main
    ```

Para practicar más a fondo, los estudiantes pueden:

- Modificar diferentes secciones del archivo simultáneamente.
- Intentar resolver conflictos más complejos, como cambios en la estructura del documento.
- Practicar el uso de `git rebase` en lugar de `git merge` para mantener un historial más limpio.

Esta práctica ayudará a los estudiantes a familiarizarse con el flujo de trabajo colaborativo en Git y GitHub, así como a manejar y resolver conflictos de manera efectiva.
