# Pokédex Angular

Aplicación web de la Pokédex construida con Angular 14. Consume la [PokéAPI](https://pokeapi.co/) (REST y GraphQL) para mostrar información, estadísticas y sprites de los Pokémon de las primeras generaciones.

La aplicación está publicada en **Azure Static Web Apps** y se actualiza automáticamente con cada push a `main` gracias a GitHub Actions.

**Sitio en producción:** <https://gentle-pebble-03dd9761e.4.azurestaticapps.net>

## Sobre el proyecto

| Dato | Valor |
|---|---|
| **Estudiante** | Milton Berrío |
| **Asignatura** | Sistemas Distribuidos |
| **Repositorio** | [MiltonBerrio/pokedex](https://github.com/MiltonBerrio/pokedex) |
| **Nube** | Microsoft Azure (suscripción gratuita) |
| **Framework** | Angular 14 |

## Crear la cuenta de Azure

Intenté usar Azure for Students, pero me daba problemas con las regiones disponibles. Al final creé una cuenta nueva de Azure independiente y activé la suscripción gratuita. Estos son los pasos que seguí:

### 1. Requisitos

- Un correo electrónico (puede ser personal, no necesita ser institucional).
- Un navegador actualizado.
- Un teléfono para la verificación en dos pasos.
- Una tarjeta de crédito o débito para verificar la identidad (Azure no cobra nada con la suscripción gratuita, solo la usa para validación).

### 2. Registro

1. Entré a [azure.microsoft.com](https://azure.microsoft.com/) y le di clic a **Empiece gratis**.
2. Inicié sesión con mi correo. Como no tenía una cuenta Microsoft asociada, tuve que crear una.
3. Azure me pidió verificar mi identidad por teléfono (SMS o llamada) y después me solicitó una tarjeta para validación.
4. Llené el formulario de contacto, acepté los términos y completé el registro.
5. Se activó la suscripción gratuita con los créditos iniciales.

### 3. Verificar la suscripción

1. Entré a [portal.azure.com](https://portal.azure.com/).
2. Busqué **Suscripciones** en la barra de búsqueda y confirmé que apareciera la suscripción gratuita con estado **Activo**.

### 4. Crear el grupo de recursos

1. En el portal, busqué **Grupos de recursos** y le di a **Crear**.
2. Seleccioné mi suscripción gratuita, escribí `rg-pokedex-production` como nombre y elegí la región **East US 2**.
3. Le di a **Revisar y crear** y luego a **Crear**.

## Despliegue

La guía completa de cómo publiqué la aplicación en Azure Static Web Apps, la configuración de encabezados de seguridad y la verificación en SecurityHeaders.com está en [Despliegue.md](Despliegue.md).

## Ejecutar el proyecto localmente

Desde la carpeta del proyecto:

```powershell
npm ci
npm start
```

Queda disponible en <http://localhost:4200/>. Para compilar en modo producción:

```powershell
npm run build
```

## Herramientas

- **Nube:** Microsoft Azure (suscripción gratuita)
- **Control de versiones:** Git y GitHub
- **Framework:** Angular 14
- **API:** [PokéAPI](https://pokeapi.co/) (REST y GraphQL)
