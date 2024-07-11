# Pedido Comida App

La aplicación Pedido Comida permite a los usuarios seleccionar y agregar productos de alimentación a su carrito de compra, ajustar la cantidad de cada artículo y revisar sus selecciones antes de confirmar el pedido. Con un proceso fluido y conveniente, los usuarios pueden editar y eliminar productos, ver un resumen de su compra y, finalmente, confirmar su pedido después de ingresar sus detalles.

## Tabla de Contenidos
- [Vista Previa](#vista-previa)
  - [Capturas de Pantalla](#capturas-de-pantalla)
  - [Enlace](#enlace)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Configuración](#configuración)
- [Uso](#uso)
- [Autor](#autor)

## Vista Previa

### Capturas de Pantalla

Pantalla de Inicio

![Pantalla de inicio](public/assets/img/screenshots/pagina_inicio.png)

Pantalla de Resumen

![Selección de productos](public/assets/img/screenshots/pagina_resumen.png)

### Enlace

- Deshabilitado temporalmente

## Tecnologías Utilizadas

- **Next.js**: Framework de React para la creación de aplicaciones web.
- **Tailwind CSS**: Framework de CSS para el diseño y estilización rápida.
- **Prisma**: ORM para interactuar con la base de datos.
- **Context API**: API de React para gestionar el estado global de la aplicación.

## Configuración

Para configurar el proyecto sigue estos pasos:

1. **Clona el repositorio**:

    ```bash
    git clone https://github.com/VmNunez/pedido-comida-app.git
    ```

2. **Instala las dependencias**:

    ```bash
    cd pedido-comida-app
    npm install
    ```

3. **Configura las Variables de Entorno**:

    Para que el proyecto funcione correctamente, es necesario configurar la variable de entorno `DATABASE_URL` en el archivo `.env`. A continuación se describe cómo hacerlo:

    1. **Crea el archivo `.env` en la raíz del proyecto** si no existe.

    2. **Configura la Variable `DATABASE_URL`**: Abre el archivo `.env` y añade la siguiente línea, reemplazando `{USUARIO}` y `{CONTRASEÑA}` con tu nombre de usuario y contraseña de la base de datos respectivamente:

        ```plaintext
        DATABASE_URL="mysql://{USUARIO}:{CONTRASEÑA}@localhost:3306/quioscoapp"
        ```

        Por ejemplo, si tu usuario es `root` y tu contraseña es `contraseña123`, la línea debería verse así:

        ```plaintext
        DATABASE_URL="mysql://root:contraseña123@localhost:3306/quioscoapp"
        ```

    #### Ejemplo Completo

    Si tienes una base de datos MySQL con los siguientes detalles:

    - **Usuario**: `root`
    - **Contraseña**: `contraseña123`
    - **Host**: `localhost`
    - **Puerto**: `3306`
    - **Nombre de la base de datos**: `quioscoapp`

    Tu archivo `.env` debería contener la siguiente línea:

    ```plaintext
    DATABASE_URL="mysql://root:contraseña123@localhost:3306/quioscoapp"
    ```

4. **Ejecuta las migraciones de la base de datos**:

    ```bash
    npx prisma migrate dev
    ```

## Uso

Para ejecutar la aplicación en un entorno de desarrollo:

```bash
npm run dev
```

## Autor
Víctor Manuel Núñez Pradas

