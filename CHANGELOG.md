# Registro de Cambios — Subsistema El Mirador

Formato basado en [Conventional Commits](https://www.conventionalcommits.org/) y
[Versionado Semántico](https://semver.org/lang/es/).

Construido colaborativamente por 3 integrantes, cada uno responsable de un
set de pantallas (ver `PROMPTS.md` para el detalle completo de prompts y
asignaciones).

## [v1.0.0] - Diseño inicial del prototipo
### feat — Integrante 1 (Login + Vista Residente)
- Pantalla de Login con accesos de demostración (RF1).
- Vista de Consulta para el Residente con datos de propiedad, bodega
  asignada y buscador de activos comunes (RF7).

### feat — Integrante 2 (Dashboard + Estado de Ocupación)
- Dashboard General con KPIs, gráfico de ocupación y actividad reciente
  (RF2, RF3).
- Módulo Estado de Ocupación con vista de gráficos y vista de tabla (RF7).

### feat — Integrante 3 (Comunidades + Torres y Bloques + Gestión de Unidades)
- Módulo Comunidades con datos oficiales del condominio.
- Módulo Torres y Bloques con vista por planta y detalle expandible (RF3).
- Módulo Gestión de Unidades con tabla de propiedades y acciones de
  ver/editar (RF3, RF7).

---

## [v1.1.0] - Correcciones de usabilidad y consistencia
### fix — Trabajo conjunto del equipo
- Se agrega breadcrumb de navegación en todas las vistas de administrador.
- Se agregan campos "Piso" y "Superficie" al modal "Registrar Nueva Unidad".
- Se convierten campos de texto libre (Torre, Propietario, Administrador)
  en selectores con datos existentes, para prevenir errores de tipeo.
- Se agrega "Recordarme" y enlace de recuperación de contraseña en Login.
- Se corrige color de texto no clicable en tabla de activos comunes de la
  Vista Residente (de azul/link a gris estándar).

### Confirmado por QA
- [x] Redirección automática por rol al iniciar sesión (RF3): probado en
      modo Presentación de Figma — admin@elmirador.cl redirige a Dashboard
      Admin, residente@elmirador.cl redirige al Portal Residente.

---

## [v1.2.0] - Pendiente
### fix / feat
- (Completar aquí si surgen nuevas correcciones tras la revisión final)
