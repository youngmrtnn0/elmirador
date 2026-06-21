# Prompts de Construcción — Subsistema El Mirador

Cada integrante ejecuta sus prompts en Figma Make, en el orden indicado.
Al terminar, cada uno sube su propia parte a GitHub con su cuenta (ver
`docs/COMO_SUBIR_A_GITHUB.md`).

---

## 🧍 Integrante 1 — Login + Vista Residente

### Prompt 1.1 — Pantalla de Login
```
Actúa como Diseñador UI/UX Senior. Diseña la pantalla de acceso (Login) del
"Subsistema de Estructura y Activos" del condominio El Mirador, usando
cuadrícula Bootstrap. Layout de dos columnas: izquierda con fondo azul
naval, logo "CONDOMINIO" con ícono de edificio, título "El Mirador" en
blanco grande, subtítulo "SUBSISTEMA DE ESTRUCTURA Y ACTIVOS", descripción
breve de "Administración integral de torres, unidades residenciales,
bodegas y activos comunes", y 3 estadísticas rápidas (Torres, Unidades,
Residentes). Columna derecha con fondo blanco: título "Ingresar al
sistema", campos "Correo electrónico" y "Contraseña" con inputs blancos de
borde sutil, botón destacado azul naval "Ingresar al Sistema" de ancho
completo, y un recuadro inferior gris claro con "Accesos de demostración"
mostrando credenciales de ejemplo para rol Administrador y Residente.
```

### Prompt 1.2 — Vista de Consulta para el Residente
```
Actúa como Diseñador UI/UX Senior. Diseña el "Portal Residente" del sistema
El Mirador, con header superior azul naval de ancho completo (sin
sidebar): logo+nombre "El Mirador / Portal Residente" a la izquierda,
nombre del usuario logueado y su rol a la derecha, junto a un botón
"Salir". Debajo, saludo personalizado "Bienvenido, [Nombre]" con subtítulo
"Información de tu propiedad y activos comunes disponibles". Sección
principal con tarjeta "Tu Propiedad" (header azul naval) mostrando Torre,
Unidad, Piso, Superficie útil, Tipo, Propietario y Estado; y tarjeta
lateral "Bodega Asignada" con ID, Ubicación, Superficie y Estado. Debajo,
dos tarjetas pequeñas de resumen (Estacionamientos de visita libres, Áreas
comunes). Al final, sección "Disponibilidad de Activos Comunes" con
buscador, filtro desplegable, y tabla con columnas ID, Torre, Tipo, Uso,
Estado — usando texto gris estándar (no azul/link) para la columna Uso.
```

### Commits sugeridos (Integrante 1)
```
feat: agrega pantalla de login con accesos demo (RF1)
feat: agrega vista de consulta para el residente (RF7)
```

---

## 🧍 Integrante 2 — Dashboard General + Estado de Ocupación

### Prompt 2.1 — Dashboard General
```
Actúa como Diseñador UI/UX Senior. Diseña el Dashboard General del
Administrador para El Mirador, con sidebar izquierdo azul naval (módulos:
Dashboard, Comunidades, Torres y Bloques, Gestión de Unidades, Estado de
Ocupación, con avatar de usuario y botón Cerrar Sesión al fondo) y topnav
superior con ícono de notificaciones (campana con badge numérico rojo) y
avatar del usuario. Contenido: título "Dashboard General", 4 tarjetas KPI
(Torres Totales, Departamentos, Bodegas, Estacionamientos) con ícono y
cifra grande. Debajo, 3 columnas: gráfico donut "Estado de Ocupación" con
buscador y filtros rápidos (Todos/Habitado/Desocupado/Mantención), gráfico
de barras "Ocupación por Torre", y lista "Actividad Reciente" con eventos
recientes con ícono y timestamp relativo. Al final, sección "Acceso Rápido
— Unidades con Atención Pendiente" con tarjetas de unidades desocupadas o
en mantención.
```

### Prompt 2.2 — Estado de Ocupación
```
Actúa como Diseñador UI/UX Senior. Diseña el módulo "Estado de Ocupación"
de El Mirador, manteniendo sidebar y topnav idénticos al Dashboard. Incluye
toggle superior derecho "Gráficos / Tabla". Vista Gráficos: 4 tarjetas de
totales (Total Activos, Habitados, Desocupados, En Mantención) con
indicador de variación, gráfico donut de distribución general, gráfico de
barras de ocupación por torre, gráfico de línea de tendencia mensual, y
barras de progreso de ocupación por tipo de activo. Vista Tabla: misma
cabecera de KPIs + buscador + tabla con columnas ID Unidad, Torre, Tipo,
Propietario, Piso, Superficie, Estado (con etiquetas de color).
```

### Commits sugeridos (Integrante 2)
```
feat: agrega dashboard general con KPIs y gráfico de ocupación (RF2, RF3)
feat: agrega módulo Estado de Ocupación con vista gráficos y tabla (RF7)
```

---

## 🧍 Integrante 3 — Comunidades + Torres y Bloques + Gestión de Unidades

### Prompt 3.1 — Comunidades
```
Actúa como Diseñador UI/UX Senior. Diseña el módulo "Comunidades" de El
Mirador, con sidebar y topnav idénticos al resto del sistema, incluyendo
breadcrumb "El Mirador > Comunidades" arriba del título. Botón destacado
"Editar Comunidad" arriba a la derecha. 4 tarjetas resumen (Torres
registradas, Total activos, Año de constitución, Residentes activos).
Debajo, tabs "Información General / Contacto y Administración /
Documentos", con la tab activa mostrando datos oficiales en grid de 2
columnas: Nombre oficial, RUT, Dirección, Comuna, Región, Código postal,
Año de constitución, Inscripción CBR, Reglamento vigente.
```

### Prompt 3.2 — Torres y Bloques
```
Actúa como Diseñador UI/UX Senior. Diseña el módulo "Torres y Bloques" de
El Mirador, con sidebar/topnav/breadcrumb idénticos al resto. Botón
"+ Registrar Torre/Bloque" arriba a la derecha. Tarjetas por torre (Torre
A, Torre B) con header azul naval mostrando nombre y badge de estado
operacional, datos de Pisos/Departamentos/Bodegas, barra de progreso de
ocupación, año de construcción, m² totales, estacionamientos,
administrador, y link "Ver detalle". Debajo, sección "Vista por Planta"
con toggle Torre A/B, mostrando unidades agrupadas por piso con etiquetas
de color según estado (Habitado verde, Desocupado gris, Mantención
amarillo), y leyenda al pie. Al expandir "Ver detalle", mostrar tarjetas
individuales por unidad con tipo, piso, m² y propietario.
```

### Prompt 3.3 — Gestión de Unidades
```
Actúa como Diseñador UI/UX Senior. Diseña el módulo "Gestión de Unidades"
de El Mirador, con sidebar/topnav/breadcrumb idénticos al resto. Botón
"+ Registrar Nueva Unidad/Bloque" arriba a la derecha. Barra de búsqueda
avanzada con filtros desplegables por Torre, Estado y Tipo. Tabla con
columnas ID Unidad, Bloque/Torre, Tipo, Propietario/Cuenta, Piso,
Superficie, Estado (etiquetas de color) y Acciones — esta última columna
con ícono de ojo (ver detalle) e ícono de lápiz (editar) por fila,
perfectamente alineados verticalmente. Incluye también el modal "Registrar
Nueva Unidad" con campos: ID Unidad, Torre/Bloque (selector), Piso,
Superficie, Propietario/Cuenta (selector), Tipo (selector) y Estado Inicial
(selector).
```

### Commits sugeridos (Integrante 3)
```
feat: agrega módulo Comunidades con datos oficiales del condominio
feat: agrega módulo Torres y Bloques con vista por planta (RF3)
feat: agrega módulo Gestión de Unidades con acciones ver/editar (RF3, RF7)
```

---

## 👥 Todos juntos — Ronda final de correcciones

Una vez que las 7 pantallas estén construidas, aplican este prompt sobre
el resultado conjunto:

```
Actúa como un Diseñador UI/UX Senior experto en QA para interfaces SaaS.
El objetivo no es crear pantallas nuevas, sino CORREGIR Y PERFECCIONAR las
pantallas existentes del sistema "El Mirador" que aún tienen errores de
usabilidad y consistencia de datos. Mantén la cuadrícula de Bootstrap y la
paleta de colores corporativos (azul naval, gris claro y blanco) en todas
las correcciones.

1. CONSISTENCIA DE NAVEGACIÓN (TODAS LAS VISTAS DE ADMINISTRADOR):
- Agrega un breadcrumb de navegación ("El Mirador > [Nombre del módulo]")
  en la parte superior de TODAS las pantallas de administrador (Dashboard,
  Torres y Bloques, Gestión de Unidades, Estado de Ocupación), usando el
  mismo estilo tipográfico y posición ya usado en la pantalla "Comunidades".
- Verifica que el topnav (ícono de campana con badge rojo + avatar "CM" de
  Carlos Morales) esté presente y sea visualmente idéntico en TODAS las
  pantallas de administrador, sin excepción.

2. CORRECCIÓN DEL MODAL "REGISTRAR NUEVA UNIDAD":
- Agrega dos campos faltantes: "Piso" (input numérico) y "Superficie"
  (input numérico con sufijo m²), ubicados después del campo "Torre/Bloque"
  y antes de "Tipo", con el mismo estilo de input y espaciado del resto
  del formulario.
- Convierte el campo "Torre/Bloque" de input de texto libre a un selector
  tipo dropdown con las opciones ya existentes en el sistema (Torre A,
  Torre B).
- Convierte el campo "Propietario/Cuenta Asociada" de input de texto libre
  a un selector tipo dropdown/autocomplete con los propietarios ya
  registrados en el sistema, para evitar errores de tipeo.

3. CORRECCIÓN DEL MODAL "REGISTRAR TORRE/BLOQUE":
- Convierte el campo "Administrador Asignado" de input de texto libre a
  un selector tipo dropdown con los administradores ya existentes en el
  sistema (ej. Carlos Morales).

4. CORRECCIÓN DE LA PANTALLA DE LOGIN:
- Agrega un checkbox "Recordarme" junto al campo de contraseña.
- Agrega un enlace de texto "¿Olvidaste tu contraseña?" alineado a la
  derecha del campo de contraseña, con estilo de texto secundario en azul
  naval, sin alterar el resto del layout del formulario.

5. CORRECCIÓN DE LA VISTA DE CONSULTA DEL RESIDENTE:
- En la tabla "Disponibilidad de Activos Comunes", cambia el color del
  texto en la columna "Uso" (valores como "Disponible" y "Estacionamiento
  Visitas") de azul (estilo de enlace) a gris/negro estándar de texto, ya
  que esos valores NO son clicables y el color azul genera una expectativa
  falsa de interactividad.

Elimina cualquier elemento de texto genérico (Lorem Ipsum) de las pantallas
corregidas y asegúrate de que cada componente se vea profesional y modular.
```

### Commits sugeridos (correcciones finales, repartidos según quién las prueba)
```
fix: agrega breadcrumb de navegación en todas las vistas de administrador
fix: agrega campos Piso y Superficie en modal Registrar Nueva Unidad
fix: convierte campos de texto libre en selectores (Torre, Propietario, Administrador)
fix: agrega "recordarme" y recuperación de contraseña en login
fix: corrige color de texto no clicable en tabla de activos comunes (vista residente)
```
