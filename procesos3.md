```mermaid
graph TD;
    A[Inicio] -->|Cliente se registra| B(Registro de Clientes);
    B -->|Cliente reserva hora| C(Registro de Reserva de Hora);
    C -->|Ingreso de proveedor| D(Registro de Proveedor);
    D -->|Registro de servicios| E(Registro de Servicios);
    E -->|Registro de orden de pedido| F(Registro de Orden de Pedido);
    F -->|Recepción de producto| G(Recepción de Producto);
    G -->|Comparar con orden de pedido| H[Coincide con la orden de pedido?];
    H -->|Sí| I(Generar factura/boleta);
    H -->|No| G;
    I -->|Gestión de empleados| J(Registro de Empleado);
    J -->|Informes y Estadísticas| K(Informes y Estadísticas);
    K -->|Administrar Boletas| L(Módulo de Administración de Boleta);
    L -->|Administrar Clientes| M(Módulo de Administración de Clientes);
    M -->|Administrar Orden de Pedido| N(Módulo de Administración de Orden de Pedido);
    N -->|Fin| O[Fin];
