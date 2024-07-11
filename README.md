# Pedido Comida App

La aplicación de Pedido Comida ofrece a los usuarios la posibilidad de seleccionar y agregar productos de alimentación a su carrito de compra, permitiéndoles ajustar la cantidad de cada artículo según sus preferencias. Después, los usuarios son dirigidos a una página de resumen de la compra, donde no solo pueden revisar sus selecciones, sino también editar la cantidad de los productos y eliminarlos si lo desean, antes de proceder al siguiente paso. Una vez satisfechos con su selección, los usuarios avanzan a la página de detalles y total, donde se calcula automáticamente el total a pagar. Después de ingresar su nombre la opción para confirmar el pedido se habilita, brindando a los usuarios un proceso fluido y conveniente para realizar sus pedidos de comida.

## Tabla de contenidos
- [Pedido Comida App](#pedido-comida-app)
  - [Tabla de contenidos](#tabla-de-contenidos)
  - [Vista Previa](#vista-previa)
    - [Capturas de pantalla](#capturas-de-pantalla)
    - [Enlace](#enlace)
  - [Tecnologías Utilizadas](#tecnologías-utilizadas)
  - [Configuración](#configuración)
  - [Uso](#uso)
  - [Autor](#autor)

## Vista Previa

### Capturas de pantalla
Pantalla de inicio

![Pantalla de inicio](public/assets/img/screenshots/pagina_inicio.png)

Pantalla de resumen

![Selección de productos](public/assets/img/screenshots/pagina_resumen.png)

### Enlace

- Deshabilitado temporalmente: [)

## Tecnologías Utilizadas

- **Next.js**: Framework de React para la creación de aplicaciones web.
- **Tailwind CSS**: Framework de CSS para el diseño y estilización rápida.
- **Prisma**: ORM para interactuar con la base de datos.
- **Context API**: API de React para gestionar el estado global de la aplicación.

## Configuración

1. Clona el repositorio:

    ```bash
    git clone https://github.com/VmNunez/pedido-comida-app.git
    ```

2. Instala las dependencias:

    ```bash
    cd pedido-comida-app
    npm install
    ```

3. Configura las variables de entorno:

    Crea un archivo `.env.local` en la raíz del proyecto y configura las siguientes variables:

    ```plaintext
    DATABASE_URL=URL_DE_TU_BASE_DE_DATOS
    ```

4. Ejecuta las migraciones de la base de datos:

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
