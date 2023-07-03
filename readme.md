### **Preguntas y Respuestas**

**Paso 11**: ¿Qué comando utilizaste? ¿Por qué?

- Comando: **`git reset --hard HEAD~1`**
- Este comando es utilizado para mover la referencia HEAD hacia atrás, específicamente un commit hacia atrás (**`HEAD~1`**). La opción **`-hard`** hace que se descarten todos los cambios no guardados en el directorio de trabajo.

**Paso 12**: ¿Qué comando o comandos utilizaste? ¿Por qué?

- Comando: **`git reflog`** y luego **`git reset --hard 8941833`**
- **`git reflog`** se utiliza para encontrar la referencia al commit al que se desea volver, en este caso, el que se deshizo en el paso anterior. Luego, con **`git reset --hard 8941833`**, se fuerza el HEAD a regresar a ese commit.

**Paso 13**: El merge, ¿Causó algún conflicto? ¿Por qué?

- No, no causó conflictos.
- Porque en la rama **`styled`** no se habían hecho cambios que afectaran las mismas líneas que los cambios realizados en la rama **`master`**.

**Paso 19**: El merge, ¿Causó algún conflicto? ¿Por qué?

- Sí, causó conflictos.
- Porque tanto la rama **`htmlify`** como la rama **`styled`** habían modificado las mismas líneas del mismo archivo.

**Paso 21**: El merge, ¿Causó algún conflicto? ¿Por qué?

- No, no causó conflictos.
- Todos los cambios de la rama **`htmlify`** ya habían sido incorporados en la rama **`styled`**.

**Paso 25**: ¿Qué comando o comandos utilizaste?

- Comando: **`git log --all --decorate --oneline --graph`**
- Este comando es utilizado para mostrar un registro de commits con en forma de ramas


**Paso 26**: El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

- Sí, podría ser "fast-forward", pero se eligió un merge "no fast-forward" para crear un nuevo commit y mantener un historial de desarrollo más claro que refleja explícitamente el proceso de fusión de la rama "title" en "master".

**Paso 27**: ¿Qué comando o comandos utilizaste?

- Comando: **`git reset --keep HEAD~1`**
- Este comando mueve la referencia HEAD hacia atrás un commit y mantiene los cambios en el directorio de trabajo.

**Paso 28**: ¿Qué comando o comandos utilizaste?

- Comando: **`git checkout -- .`**
- Este comando descarta todos los cambios en el directorio de trabajo que aún no se han añadido al área de preparación.

**Paso 29**: ¿Qué comando o comandos utilizaste?

- Comando: **`git branch -d title`** y luego **`git branch -D title`** si es necesario.
- Primero se intenta eliminar la rama **`title`** con **`git branch -d title`**. Si la rama **`title`** no está completamente fusionada y aún así se quiere utilizar, se utiliza el comando **`git branch -D title`**. Esto forzará la eliminación de la rama **`title`** sin importar su estado.

**Paso 30**: ¿Qué comando o comandos utilizaste?

- Comando: **`git reflog`** y luego **`git reset --hard 0246bf2`**
- Este comando es utilizado para regresar a un commit específico, descartando todos los cambios que ocurrieron después de ese commit. En este caso, se usa el hash del commit (0246bf2) que corresponde al estado después de hacer el merge entre la rama "master" y "title". La opción **`--hard`** asegura que los cambios en el directorio de trabajo se descarten para que coincidan exactamente con el estado del commit.

**Paso 32**: ¿Qué comando o comandos utilizaste?

 - Comando: **`git checkout 6114af4240a2adfd8332fe48bde78bf2695c8e71`**
 - Este commit corresponde al commit inicial cuando se creó el poema.

**Paso 33**: ¿Qué comando o comandos usaste?

- Comando: **`git reset --hard 297acf969bafc64420bf8bce0f6c737a6b765381 `**
