## Agenda de la Clase

1. **Introducción a Git Flow**

   - ¿Qué es Git Flow y por qué se usa en entornos de desarrollo?
   - Principales ramas en Git Flow: `main`, `develop`, `feature`, `release`, `hotfix`.

2. **Comandos Básicos de Git Flow**

   - ¿Cómo se inicializa Git Flow en un proyecto?
   - Principales comandos de Git Flow (`start`, `finish`).

3. **Flujo de Trabajo de Git Flow**

   - Creación y finalización de `feature`.
   - Creación y finalización de `release`.
   - Creación y finalización de `hotfix`.

4. **Fusiones y Resolución de Conflictos**

   - ¿Cómo se manejan las fusiones automáticas?
   - Resolución de conflictos en ramas de `feature`, `release` y `hotfix`.

5. **Práctica y Ejercicios Guiados**
   - Ejercicio de creación de ramas `feature`.
   - Ejercicio de simulación de conflictos.
   - Ejercicio de finalización de una `release`.

---

## Preguntas para la Clase

### 1. Introducción a Git Flow

- **¿Qué es Git Flow?**  
  Es una metodología para gestionar ramas en Git, que organiza el desarrollo en ramas específicas para `main`, `develop`, `feature`, `release` y `hotfix`.

- **¿Cuáles son las principales ventajas de usar Git Flow en un proyecto?**  
  Permite un control más organizado y seguro de las versiones de producción, desarrollo, y de las funcionalidades nuevas, además de simplificar la colaboración en equipo.

### 2. Comandos Básicos

- **¿Cómo se inicia Git Flow en un proyecto?**  
  Con el comando `git flow init`.

- **¿Qué comando se usa para iniciar una nueva rama de `feature`?**  
  `git flow feature start <nombre_feature>`.

- **¿Cómo se finaliza una rama de `feature` y qué sucede con ella?**  
  `git flow feature finish <nombre_feature>`. Git Flow fusiona automáticamente la `feature` en `develop` y elimina la rama de `feature`.

### 3. Flujo de Trabajo

- **¿Cuál es el propósito de la rama `develop`?**  
  `develop` es la rama donde se integran todas las nuevas funcionalidades (features) para pruebas e integración, antes de una `release`.

- **¿Qué es una `release` y cómo se crea en Git Flow?**  
  Una `release` es una rama creada para preparar una versión de producción del proyecto; se inicia con `git flow release start <versión>`.

- **¿Para qué se usa una rama de `hotfix` y cómo se finaliza?**  
  Un `hotfix` se usa para realizar una corrección urgente en la versión de producción (`main`). Se finaliza con `git flow hotfix finish <nombre_hotfix>`, fusionando los cambios en `main` y `develop`.

### 4. Fusiones y Conflictos

- **¿Cómo fusiona automáticamente Git Flow las ramas al finalizar una `feature` o `release`?**  
  Git Flow usa fusiones automáticas sin fast-forward, lo que crea un commit de fusión que mantiene el historial del cambio.

- **¿Qué pasos debes seguir si encuentras un conflicto durante una fusión?**  
  Editar los archivos en conflicto, resolver las diferencias, agregar los cambios con `git add`, y realizar el commit final para completar la fusión.

### 5. Ejercicios

Para reforzar los conceptos, practica con estos ejercicios:

- **Ejercicio 1**: Crea una nueva rama de `feature`, realiza algunos commits y finaliza la `feature`.
- **Ejercicio 2**: Inicia una rama de `release`, realiza algunos cambios y luego finalízala.
- **Ejercicio 3**: Crea un `hotfix` a partir de `main`, haz una corrección urgente y finalízalo.
- **Ejercicio 4**: Simula un conflicto al modificar el mismo archivo en una `feature` y en `develop`. Resuelve el conflicto y completa la fusión.

---

¡Buena práctica y disfruta aprendiendo Git Flow!
