# Tu Ferretería - Aplicación Móvil

## Descripción

"**Tu Ferretería**" es una aplicación móvil diseñada para gestionar de manera eficiente los productos y compras en la ferretería. La aplicación está destinada a ser utilizada exclusivamente para esta ferretería, lo que la convierte en una solución personalizada y **ad hoc**. Utilizando **Flutter** y **Dart**, la aplicación se conecta a un servidor externo para manejar la persistencia de datos mediante **Supabase**.

---

## Funcionalidades

### **Autenticación de Usuarios**
- Usa **Supabase Auth** para permitir registro y login.
- Los usuarios tendrán sesiones persistentes, con pantallas dedicadas para el inicio de sesión y registro.

### **Gestión de Roles**
- Administra roles desde Supabase para diferenciar entre administradores y clientes.
- Los **administradores** gestionan productos e inventarios, mientras los **clientes** realizan compras.

### **Crear Producto**
- Pantalla donde el **administrador** puede ingresar el nombre, descripción, precio, cantidad y subir una imagen del producto.
- Incluye validaciones y un botón para confirmar la creación del producto.

### **Editar Producto**
- Permite modificar la información de productos existentes.
- Carga los datos actuales del producto en un formulario editable y actualiza la base de datos al guardar los cambios.

### **Ver Carrito**
- Pantalla donde el **cliente** puede ver los productos agregados a su carrito, ajustar cantidades, eliminar artículos y proceder al pago.
- Muestra el total actualizado en tiempo real.

### **Historial de Carrito**
- Muestra un listado de pedidos realizados por el **cliente**, con detalles de cada pedido, como fecha, productos comprados, cantidad y precio total.
- Incluye una vista detallada para cada compra.

---

## Arquitectura

La aplicación está construida utilizando una **arquitectura distribuida**. Los datos se gestionan en un **servidor externo** a través de **Supabase**, que proporciona tanto la autenticación como la base de datos necesaria para la aplicación.

---

## Tecnologías Utilizadas

- **Flutter**: Framework para la creación de interfaces móviles.
- **Dart**: Lenguaje de programación utilizado para desarrollar la aplicación.
- **Supabase**: Plataforma que proporciona autenticación, base de datos y almacenamiento en tiempo real.
- **PostgreSQL**: Sistema de gestión de bases de datos utilizado por Supabase para manejar los datos de la aplicación.

---

## Instalación

### **Requisitos Previos**
- Tener instalado [Flutter](https://flutter.dev/docs/get-started/install).
- Tener una cuenta en [Supabase](https://supabase.io/).
- Tener instalado [AndroidStudio](https://developer.android.com/)

### **Pasos de Instalación**
1. Clona este repositorio en tu máquina local:

   ```bash
   git clone https://github.com/DOKG0/FerreteriaApp.git
