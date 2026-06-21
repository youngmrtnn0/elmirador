# Subsistema de Estructura y Activos — El Mirador

Prototipo funcional en Figma para la administración de torres, unidades residenciales,
bodegas y activos comunes del condominio El Mirador.

## 🔗 Prototipo
- **Figma (vista):** [pega aquí el link público de Figma]
- **Herramienta de prototipado:** Figma (Figma Make)

## 📦 Entregables de este repositorio
- `/docs` → Plan de pruebas (ISO 25000), Planilla de Nielsen, Registro de pruebas
- `/assets` → Capturas de cada versión del prototipo, organizadas por integrante/versión
- `PROMPTS.md` → Prompts usados para construir cada pantalla, divididos por integrante
- `CHANGELOG.md` → Registro de control de cambios con versionado semántico

## 🧭 Estrategia de control de versiones

Usamos **Versionado Semántico (SemVer)** + **Conventional Commits**:

```
MAYOR.MENOR.PARCHE   →   ej. v1.1.0
```
- **MAYOR**: cambios que rompen estructura/flujo existente
- **MENOR**: nuevas pantallas o módulos agregados
- **PARCHE**: correcciones de bugs/usabilidad sin agregar funcionalidad nueva

### Prefijos de commit usados
| Prefijo | Uso |
|---|---|
| `feat:` | Nueva pantalla o funcionalidad |
| `fix:` | Corrección de error de usabilidad/funcionalidad |
| `style:` | Cambios visuales sin alterar funcionalidad |
| `docs:` | Cambios en documentación (plan de pruebas, Nielsen, etc.) |
| `refactor:` | Reestructuración de componentes sin cambiar comportamiento |

## 👥 Equipo y responsabilidades
| Integrante | Pantallas a cargo |
|---|---|
| [Nombre 1] | Login, Vista Residente |
| [Nombre 2] | Dashboard General, Estado de Ocupación |
| [Nombre 3] | Comunidades, Torres y Bloques, Gestión de Unidades |

Ver `PROMPTS.md` para el detalle de cada prompt usado y los commits
sugeridos por integrante.
