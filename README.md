Sistema de Gestión de Usuarios y Productos Veterinaria - Atacama Pets

Para este proyecto se tiene contemplado desarrollar una aplicación web tipo intranet, diseñada para optimizar y digitalizar los procesos operativos de la clínica veterinaria Atacama Pets. para esta evaluacion solo se sentrara en el historial clinicos de pacientes ademas del control de inventario médico, asegurando la integridad de los datos y restringiendo el acceso únicamente a personal autorizado.


Se utilizaron las siguientes herramientas:

1.Framework Base: Next.js (entorno React).

2.Lenguaje(TypeScript): Para garantizar una consistencia estructural de los datos.

3.UseContext: para el manejo global de la sesión del usuario.

4.LocalStorage: para el almacenamiento temporal y estructurado de la información.

Entre los Módulos implementados se encuentran:

1. Módulo de Autenticación y Seguridad
-Validación de credenciales mediante un formulario.
-Implementación de un componente de orden superior (RutaProtegida) para asegurar las rutas internas y se ejecuten la redirección automática de usuarios no autenticados.

2. Panel de Control (Dashboard)
-Interfaz principal de navegación post-autenticación.
-Identificación dinámica del usuario activo y su rol correspondiente dentro de la clínica.
- Enrutamiento declarativo hacia los módulos operativos.

3. Módulo de Gestión de Pacientes (CRUD)
-Creación y Edición: Registro de mascotas con validación estricta de entradas en el formulario (prevención de caracteres no seguros y control de formato en los campos numéricos como RUT y Edad).
-Búsqueda: Filtro indexado en tiempo real por el nombre del paciente.
-Eliminación: Borrado de registros del sistema con confirmación previa.

4. Módulo de Control de Inventario (CRUD)
-Administración del stock de insumos, alimentos y medicamentos.

-Registro de entidades con atributos específicos: código, nombre, categoría, stock, precio y fecha de caducidad.

-Capacidad de actualización de existencias y eliminación de ítems del catálogo.