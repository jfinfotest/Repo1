# Proyecto WEB



| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

<details>

<summary>Tips for collapsed sections</summary>

### You can add a header

You can add text within a collapsed section.

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```

</details>

```js
function test() {
  console.log("notice the blank line before this function?");
}
```

#  Semana 5 - Fundamentación de los Sistemas de Control de Versiones

## ¿Qué son?

Los sistemas de control de versiones (SCV) son herramientas que permiten el seguimiento y la gestión de cambios en archivos o conjuntos de archivos a lo largo del tiempo. Permiten:

-   Registrar las modificaciones: Cada cambio realizado en un archivo se guarda como una nueva versión, creando un historial completo del desarrollo.
-   Recuperar versiones anteriores: Si se comete un error o se desea volver a una versión anterior del proyecto, es posible hacerlo con facilidad.
-   Colaborar en equipo: Los SCV facilitan el trabajo en equipo, permitiendo a varios usuarios trabajar en el mismo proyecto de forma simultánea y sincronizada.
-   Compartir el código: Los SCV permiten compartir el código de forma pública o privada, facilitando la colaboración con otros desarrolladores.

## Beneficios

-   Mejora la calidad del código: Permite realizar un seguimiento de los cambios y revertir errores fácilmente.
-   Facilita la colaboración: Permite trabajar en equipo de forma eficiente y segura.
-   Aumenta la productividad: Ahorra tiempo al evitar la duplicación de trabajo y la pérdida de datos.
-   Mejora la comunicación: Permite a los desarrolladores comprender mejor la evolución del proyecto.
-   Promueve la transparencia: Permite a todos los miembros del equipo tener acceso al historial del proyecto.

## ¿Qué es Git?

Git es un sistema de control de versiones distribuido, de código abierto y gratuito, utilizado para el seguimiento y la gestión de cambios en archivos o conjuntos de archivos.

### Beneficios de usar Git

-   Control de versiones: Permite realizar un seguimiento de todos los cambios realizados en el proyecto.
-   Colaboración: Permite trabajar en equipo de forma eficiente y segura.
-   Reversibilidad: Permite volver a una versión anterior del proyecto en caso de errores.
-   Eficiencia: Ahorra tiempo al evitar la duplicación de trabajo y la pérdida de datos.
-   Flexibilidad: Permite trabajar con diferentes branches y realizar merges de forma sencilla.
-   Seguridad: Protege los archivos contra la pérdida accidental o la corrupción.

### Flujo de trabajo en Git

![https://neurathsboat.blog/post/git-intro/img/Git_trees.png](https://neurathsboat.blog/post/git-intro/img/Git_trees.png)


### Comandos de configuración inicial de Git

Al iniciar con Git, hay algunos comandos que puedes usar para personalizar tu experiencia y optimizar tu flujo de trabajo. Estos son algunos de los comandos más comunes para la configuración inicial:

Configurar tu nombre y correo electrónico:

-   `git config --global user.name "Tu nombre completo"`: Establece tu nombre de usuario global.
-   `git config --global user.email "tucorreo@email.com"`: Establece tu correo electrónico global.

Ejemplos:

-   Para establecer el nombre de usuario global:

```bash
git config --global user.name "Juan Pérez"
git config --global user.email "juanperez@gmail.com"

```
-   Para mostrar todas las configuraciones:

```bash
git config --list
```

### El comando git --version

Se utiliza para verificar qué versión de Git está instalada.

```bash   
git --version
```

### Comandos de básicos de Git

#### `git init`

Este comando crea un nuevo repositorio Git en el directorio actual. Un repositorio Git es una carpeta que contiene el historial de commits, las ramas y la configuración del proyecto.

Ejemplo:

```bash
mkdir mi_proyecto
cd mi_proyecto
git init

```

Explicación:

-   `mkdir mi_proyecto`: Crea una nueva carpeta llamada `mi_proyecto`.
-   `cd mi_proyecto`: Cambia el directorio actual a `mi_proyecto`.
-   `git init`: Inicializa un nuevo repositorio Git en la carpeta `mi_proyecto`.

Resultado:

-   Se crea un archivo `.git` en la carpeta `mi_proyecto`. Este archivo contiene metadatos sobre el repositorio, como el historial de commits y la configuración.

#### `git add`

Este comando agrega archivos al área de preparación para el siguiente commit. El área de preparación es un espacio temporal donde se almacenan los cambios antes de ser confirmados en el historial del proyecto.

Ejemplo:

```bash
git add archivo.txt

```

Explicación:

-   `git add archivo.txt`: Agrega el archivo `archivo.txt` al área de preparación.

Resultado:

-   El archivo `archivo.txt` se marca como listo para ser incluido en el siguiente commit.

#### `git add .`

El comando git add . en Git se utiliza para agregar todos los archivos modificados y no rastreados en tu directorio actual al área de preparación para la siguiente confirmación (commit).

```bash
git add .

```

#### `git commit`

Este comando crea un commit con los cambios del área de preparación. Un commit es una instantánea permanente del estado del proyecto en un momento determinado.

Ejemplo:

```bash
git commit -m "Mensaje del commit"

```

Explicación:

-   `git commit`: Crea un commit con los cambios del área de preparación.
-   `-m "Mensaje del commit"`: Especifica un mensaje que describe los cambios en el commit.

Resultado:

-   Se crea un nuevo commit en el historial del proyecto. El commit contiene los cambios que se agregaron al área de preparación.

#### `git commit -am`

El comando git commit -am "mensaje" en Git es una forma abreviada de confirmar tus cambios junto con un mensaje de confirmación. 

```bash
git commit -am "Mensaje del commit"

```

#### `git clone`

Este comando clona un repositorio remoto en tu equipo local. Crea una copia del repositorio en tu computadora para que puedas trabajar en él.

Ejemplo:

```bash
git clone https://url_del_repositorio.git

```

Explicación:

-   `git clone https://url_del_repositorio.git`: Clona el repositorio remoto ubicado en `https://url_del_repositorio.git` en la carpeta actual.

Resultado:

-   Se crea una copia del repositorio remoto en la carpeta actual.
-   La copia local del repositorio está sincronizada con la versión remota.

#### `git push`

Este comando envía los cambios locales al repositorio remoto. Sube tus cambios al repositorio para que otros puedan acceder a ellos.

Ejemplo:

```bash
git push

```

Explicación:

-   `git push`: Envía los cambios locales al repositorio remoto.

Resultado:

-   Los cambios que se han confirmado en la rama actual se envían al repositorio remoto.
-   La versión remota del repositorio se actualiza con los cambios locales.

#### `git pull`

-   La versión local del repositorio se actualiza con los últimos cambios del repositorio remoto.

Ejemplo:

```bash
git pull

```

## Que es Github?

### GitHub se puede entender como dos cosas:

1.  Almacenamiento de código con control de versiones: En esencia, GitHub es una plataforma en la nube que permite a los desarrolladores alojar sus proyectos de código fuente. Funciona utilizando un sistema de control de versiones llamado Git, que realiza un seguimiento de todos los cambios realizados en el código a lo largo del tiempo. Esto permite a los desarrolladores volver a versiones anteriores del código si es necesario, y colaborar fácilmente en proyectos con otros.

2.  Plataforma para colaboración: GitHub va más allá del simple almacenamiento de código. Ofrece una variedad de herramientas que facilitan la colaboración entre desarrolladores. Estas herramientas incluyen:

    -   Control de acceso: Puedes establecer permisos para controlar quién puede ver y modificar el código de tu proyecto.
    -   Problema de seguimiento: Puedes crear y rastrear errores y tareas pendientes relacionadas con tu proyecto.
    -   Solicitudes de extracción (Pull requests): Esta función permite a los desarrolladores proponer cambios al código de un proyecto para que sean revisados y fusionados por otros colaboradores.
    -   Wikis del proyecto: Crea documentación y notas compartidas para tu proyecto.

### Flujo básico de trabajo en GitHub:

1.  Clonar un repositorio: Descarga una copia del proyecto de GitHub a tu computadora.
2.  Crear una rama: Crea una nueva rama para trabajar en tu propio conjunto de cambios.
3.  Realizar cambios: Edita los archivos del proyecto y haz cambios localmente.
4.  Confirmar cambios: Guarda los cambios en tu repositorio local con un mensaje descriptivo.
5.  Subir cambios: Sube tus cambios al repositorio remoto en GitHub.
6.  Enviar una solicitud de extracción (Pull request): Propón tus cambios para que sean revisados y fusionados en la rama principal del proyecto.

Comandos básicos en Git:

-   `git init`: Crea un nuevo repositorio Git en la carpeta actual.
-   `git clone`: Descarga un repositorio remoto a tu computadora.
-   `git add`: Agrega archivos al índice de Git para ser confirmados.
-   `git commit`: Guarda los cambios en el índice como un nuevo commit.
-   `git push`: Sube tus cambios al repositorio remoto.
-   `git pull`: Descarga los cambios del repositorio remoto y fusiona con tu rama local.

### Git Pages 

Git Pages es una funcionalidad que ofrece GitHub para hospedar tu sitio web directamente desde tu repositorio de GitHub una referencia en español: una referencia en español sobre Git Pages. Proporciona una manera gratuita y fácil de publicar sitios web estáticos.

Aquí algunos puntos clave sobre Git Pages:

-   **Sitios web estáticos:** Solo puede alojar sitios web estáticos, lo que significa que el contenido de tu sitio web está preconstruido con archivos HTML, CSS y JavaScript.
-   **Flujo de trabajo simple:** Los cambios que realices en los archivos de tu sitio web se reflejan en vivo en tu sitio una vez que los subas a tu repositorio de GitHub. Esto facilita mucho la implementación de actualizaciones en tu sitio web.
-   **Gratuito:** Git Pages es completamente gratuito para repositorios públicos. También hay planes pagos para repositorios privados.
-   **Personalización:** Puedes personalizar la apariencia de tu sitio web usando temas o creando tu propio HTML y CSS.


## Tutorial de manejo de branches en Git y GitHub

Este tutorial te guiará en el manejo de branches en Git y GitHub, cubriendo desde lo básico hasta conceptos avanzados.

### 1. Conceptos básicos

* **Repositorio:** Un repositorio Git es una carpeta que contiene todos los archivos de un proyecto, junto con el historial de cambios.
* **Branch:** Una branch es una copia independiente del repositorio, permitiendo trabajar en nuevas funcionalidades sin afectar el código principal.
* **Master (main):** La branch principal, donde se almacenan las versiones estables del proyecto.
* **Commit:** Una confirmación de los cambios realizados en el repositorio, creando un punto de referencia en el historial.

### 2. Creando y manejando branches

**2.1 Creando una nueva branch:**

```bash
git checkout -b <nombre_de_branch> 
```

Ejemplo: `git checkout -b feature-login` crea una nueva branch llamada "feature-login".

**2.2 Listando las branches:**

```bash
git branch
```

**2.3 Cambiando de branch:**

```bash
git checkout <nombre_de_branch>
```

**2.4 Fusionando branches:**

```bash
git checkout master
git merge <nombre_de_branch>
```

**2.5 Eliminando una branch:**

```bash
git branch -d <nombre_de_branch>
```

**2.6 Resolviendo conflictos:**

Si las dos branches que se fusionan tienen cambios en los mismos archivos, Git mostrará un conflicto. Deberás editar el archivo manualmente y luego usar:

```bash
git add <archivo_conflictivo>
git commit -m "Resuelto conflicto en <archivo>"
```

### 3. Trabajando con GitHub

**3.1 Creando un repositorio en GitHub:**

Crea un nuevo repositorio en GitHub y copia la URL.

**3.2 Clonar el repositorio:**

```bash
git clone <URL_del_repositorio>
```

**3.3 Push y Pull:**

* **Push:**  Envía los cambios de tu branch local al repositorio remoto en GitHub.
```bash
git push origin <nombre_de_branch>
```
* **Pull:** Descarga los cambios del repositorio remoto a tu branch local.
```bash
git pull origin <nombre_de_branch>
```

**3.4 Creando una Pull Request (PR):**

* Crea una nueva PR desde tu branch en GitHub.
* Describe los cambios y solicita revisión por parte de otros colaboradores.
* Una vez aprobada, se fusiona la PR a la branch principal.

---

## **Tutorial: Git, GitHub y Despliegue en GitHub Pages**

## **Objetivo**
Aprenderás cómo:
1. Inicializar un repositorio Git.
2. Conectar tu proyecto local con GitHub.
3. Hacer commits y subir cambios a GitHub.
4. Desplegar tu proyecto web en GitHub Pages.

---

## Estructura del proyecto

```
/proyecto-integrador
│
├── /src                     # Carpeta principal para el código fuente
│   ├── /assets              # Archivos estáticos (imágenes, fuentes, etc.)
│   │   ├── /images          # Imágenes utilizadas en el proyecto
│   │   ├── /fonts           # Fuentes personalizadas
│   │   └── /icons           # Iconos (SVG, PNG, etc.)
│   │
│   ├── /css                 # Archivos CSS
│   │   ├── styles.css       # Estilos globales
│   │   ├── reset.css        # Reset de estilos (opcional)
│   │   └── pages.css        # Estilos específicos para páginas
│   │
│   ├── /js                  # Archivos JavaScript
│   │   ├── main.js          # Punto de entrada principal del proyecto
│   │   └── utils.js         # Funciones utilitarias reutilizables
│   │
│   ├── /pages               # Archivos HTML específicos para páginas
│       ├── home.html        # Página de inicio
│       └── about.html       # Página "Acerca de"
│  │
├── index.html               # Página principal del proyecto
├── README.md                # Documentación del proyecto
```

## **Paso 1: Configuración inicial de Git**

Antes de comenzar, asegúrate de tener instalado **Git** en tu computadora. Puedes descargarlo desde [git-scm.com](https://git-scm.com/).

### **1.1 Verifica la instalación de Git**
Abre una terminal (Command Prompt, PowerShell o Terminal) y ejecuta el siguiente comando:
```bash
git --version
```
Si ves algo como `git version X.XX.X`, significa que Git está instalado correctamente.

### **1.2 Configura tu nombre y correo electrónico**
Estos datos se usarán para identificar tus commits. Ejecuta los siguientes comandos:
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu.correo@example.com"
```

---

## **Paso 2: Crear un repositorio local**

### **2.1 Navega al directorio del proyecto**
Supongamos que tu proyecto está en la carpeta `/proyecto-web`. Abre la terminal y navega hasta esa carpeta:
```bash
cd ruta/a/tu/proyecto-web
```

### **2.2 Inicializa el repositorio**
Ejecuta el siguiente comando para inicializar un repositorio Git en tu proyecto:
```bash
git init
```
Esto creará una carpeta oculta llamada `.git` en tu proyecto, que almacenará todo el historial de cambios.

---

## **Paso 3: Crear un repositorio en GitHub**

### **3.1 Crea una cuenta en GitHub**
Si no tienes una cuenta, regístrate en [github.com](https://github.com/).

### **3.2 Crea un nuevo repositorio**
1. Haz clic en el botón **"New"** en la página principal de GitHub.
2. Asigna un nombre al repositorio (por ejemplo, `proyecto-web`).
3. Deja las opciones predeterminadas (público o privado, según prefieras).
4. **No inicialices el repositorio con un README** porque ya lo harás localmente.

---

## **Paso 4: Conectar el repositorio local con GitHub**

### **4.1 Copia la URL del repositorio**
En la página de tu repositorio recién creado, copia la URL HTTPS (se verá algo como `https://github.com/tu-usuario/proyecto-web.git`).

### **4.2 Agrega el repositorio remoto**
En tu terminal, ejecuta el siguiente comando para conectar tu proyecto local con GitHub:
```bash
git remote add origin https://github.com/tu-usuario/proyecto-web.git
```

---

## **Paso 5: Realizar tu primer commit**

### **5.1 Añade todos los archivos al área de preparación**
Ejecuta el siguiente comando para añadir todos los archivos de tu proyecto al área de preparación:
```bash
git add .
```

### **5.2 Realiza el commit**
Crea un commit con un mensaje descriptivo:
```bash
git commit -m "Primer commit: Estructura inicial del proyecto"
```

### **5.3 Sube los cambios a GitHub**
Sube los cambios al repositorio remoto en GitHub:
```bash
git branch -M main
git push -u origin main
```
Esto enviará tu código a la rama `main` de tu repositorio en GitHub.

---

## **Paso 6: Desplegar el proyecto en GitHub Pages**

GitHub Pages permite alojar sitios web directamente desde un repositorio. Sigue estos pasos:

### **6.1 Asegúrate de que tu proyecto tenga un archivo `index.html`**
El archivo `index.html` en la raíz de tu proyecto será la página principal de tu sitio web. Si usaste la estructura anterior, ya deberías tener este archivo en `/src/index.html`.

### **6.2 Cambia la estructura si es necesario**
GitHub Pages requiere que el archivo `index.html` esté en la raíz del repositorio. Si tu archivo está en `/src`, mueve toda la carpeta `/src` a la raíz del proyecto:
```
mv src/* .
```

### **6.3 Activa GitHub Pages**
1. Ve a la página de tu repositorio en GitHub.
2. Haz clic en la pestaña **Settings** (Configuración).
3. En el menú lateral, selecciona **Pages**.
4. En la sección **Source**, selecciona la rama `main` y la carpeta `/root`.
5. Haz clic en **Save**.

GitHub generará automáticamente una URL para tu sitio web. Por ejemplo:
```
https://tu-usuario.github.io/proyecto-web/
```

### **6.4 Espera a que se publique**
GitHub tardará unos minutos en procesar tu sitio. Una vez listo, verás un mensaje indicando que tu sitio está publicado.

---

## **Paso 7: Actualizar el proyecto**

Si realizas cambios en tu proyecto, sigue estos pasos para actualizar el repositorio y el sitio web:

### **7.1 Añade los cambios**
```bash
git add .
```

### **7.2 Realiza un commit**
```bash
git commit -m "Descripción de los cambios realizados"
```

### **7.3 Sube los cambios a GitHub**
```bash
git push origin main
```

### **7.4 Verifica el sitio actualizado**
Visita la URL de GitHub Pages para ver los cambios reflejados.

---

3. **Colabora con otros:**
   Si trabajas en equipo, usa Pull Requests en GitHub para revisar y fusionar cambios.

---

## **Resumen de comandos útiles**

| Comando                     | Descripción                                      |
|-----------------------------|--------------------------------------------------|
| `git init`                  | Inicializa un repositorio Git.                  |
| `git add .`                 | Añade todos los archivos al área de preparación.|
| `git commit -m "mensaje"`   | Guarda los cambios con un mensaje descriptivo.  |
| `git push origin main`      | Sube los cambios a la rama `main` en GitHub.    |
| `git pull origin main`      | Descarga los cambios más recientes de GitHub.   |

---

