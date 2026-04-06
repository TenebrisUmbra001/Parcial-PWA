Sistema de Gestión de Turnos

Aplicación web  para la gestión de reservas de turnos. Desarrollada como proyecto de evaluación para demostrar el manejo de React, enrutamiento, estado global y validaciones de negocio del lado del cliente.
🚀 Características

    Gestión de Turnos: Alta, baja y modificación de turnos con control de horarios y capacidades.
    Sistema de Reservas: Los usuarios pueden reservar cupos en tiempo real con validación de disponibilidad.
    Panel Administrativo: Área protegida para gestionar el flujo completo del sistema.
    Persistencia de Datos: Utiliza localStorage para simular una base de datos, manteniendo la información entre recargas de página.
    Validaciones de Negocio Robustas:
        Detección de solapamiento de horarios (evitando crear turnos que choquen).
        Protección de integridad: No permite editar turnos que ya tienen reservas confirmadas.
        No permite borrar turnos con datos asociados.
        Control estricto de cupos máximos.

🛠️ Tecnologías Utilizadas

    React 18 (vía CDN)
    React Router DOM 6 (Enrutamiento anidado y protegido)
    Babel (Transpilación de JSX en el navegador)
    HTML5 & CSS3 (Diseño Responsive y CSS Variables)

📋 Requisitos Previos

Este proyecto está diseñado para ejecutarse directamente en el navegador. No requiere instalación de Node.js ni dependencias.


👤 Credenciales de Acceso (Demo) 

Para acceder al panel administrativo y probar la gestión completa, utiliza las siguientes credenciales pre-cargadas en el sistema: 

     Email: admin@turnos.com
     Contraseña: 123
     

📂 Estructura del Código 

El proyecto se encuentra contenido en un único archivo index.html para facilitar su portabilidad y evaluación. Sin embargo, el código interno está organizado modularmente: 

     Capa de Presentación: Componentes React (Login, CRUDTurnos, TurnosDisponibles, etc.).
     Capa de Lógica (Custom Hooks):
         useAuth: Manejo de autenticación y rutas protegidas.
         useStorage: Abstracción sobre localStorage para persistencia de datos.
         useTurnos: Lógica de negocio compleja (validaciones de horarios, solapamientos).
         useReservas: Lógica de reservas y verificación de cupos.
         
     Enrutamiento: Configuración de rutas anidadas y públicas usando React Router.
     
