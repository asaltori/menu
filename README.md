# Plataforma de Restaurante Multi-Carrito

Esta es una plataforma web desarrollada en React que permite a un restaurante gestionar un menú dinámico compuesto por múltiples carritos de comida externos.

## Características

- **Menú Dinámico**: Los carritos gestionan sus platos y costos.
- **Estrategia de Precios**: El restaurante define el precio final de venta.
- **Pedidos QR**: Los clientes escanean un QR único por mesa para ordenar.
- **Roles de Usuario**:
  - **Administrador**: Gestión global y generación de QRs.
  - **Carrito**: Gestión de disponibilidad de platos y costos.
  - **Restaurante**: Fijación de precios y monitoreo de envíos.
  - **Camarero**: Confirmación y modificación de órdenes.
  - **Cliente**: Visualización de menú y pedidos.

## Instalación y Ejecución

Este proyecto utiliza Vite. Asegúrate de tener Node.js instalado.

1.  Instalar dependencias:
    ```bash
    npm install
    ```

2.  Iniciar el servidor de desarrollo:
    ```bash
    npm run dev
    ```

3.  Abrir en el navegador (usualmente http://localhost:5173).

## Estructura del Proyecto

- `src/context/StoreContext.jsx`: Simula la base de datos y la lógica de negocio.
- `src/pages/`: Contiene las vistas para cada rol.
- `src/components/`: Componentes reutilizables como el Layout.

## Uso (Simulación)

Al iniciar la aplicación, verás una pantalla de Login simulada. Puedes hacer clic en cualquiera de los usuarios predefinidos para acceder a su dashboard correspondiente.

- **Admin**: Genera QRs para las mesas.
- **Carrito**: Activa/desactiva platos y cambia sus costos.
- **Restaurante**: Define el precio de venta al público.
- **Cliente**: Simula el escaneo de QR accediendo a "Acceso Clientes".
