```mermaid
graph TD;
    A[Inicio] -->|Cliente se registra| B(Registro de Clientes);
    B -->|Cliente reserva hora| C(Registro de Reserva de Hora);
    C -->|Ingreso de proveedor| D(Registro de Proveedor);
    D -->|Registro de servicios| E(Registro de Servicios);
    E -->|Registro de orden de pedido| F(Registro de Orden de Pedido);
    F -->|Recepción de producto| G(Recepción de Producto);
    G -->|Generar factura/boleta| H(Registro Factura/Boleta);
    H -->|Gestión de empleados| I(Registro de Empleado);
    I -->|Informes y Estadísticas| J(Informes y Estadísticas);
    J -->|Administrar Boletas| K(Módulo de Administración de Boleta);
    K -->|Administrar Clientes| L(Módulo de Administración de Clientes);
    L -->|Administrar Orden de Pedido| M(Módulo de Administración de Orden de Pedido);
    M -->|Fin| N[Fin];
