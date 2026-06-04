# 📘 Manual de Usuario — ATLAS

**Herramienta Adaptativa para Auditoría Legislativa y Estándares**

> **Versión:** 1.0  
> **Fecha:** Junio 2026  
> **Plataforma:** Aplicación Web (Angular 21)

---

## Tabla de Contenidos

1. [Introducción](#1-introducción)
2. [Requisitos del Sistema](#2-requisitos-del-sistema)
3. [Acceso a la Plataforma](#3-acceso-a-la-plataforma)
   - 3.1 [Página de Inicio (Landing Page)](#31-página-de-inicio-landing-page)
4. [Registro de Usuario](#4-registro-de-usuario)
   - 4.1 [Crear una Cuenta](#41-crear-una-cuenta)
   - 4.2 [Activación de Cuenta](#42-activación-de-cuenta)
   - 4.3 [Establecer Contraseña](#43-establecer-contraseña)
   - 4.4 [Reenviar Correo de Activación](#44-reenviar-correo-de-activación)
5. [Inicio de Sesión](#5-inicio-de-sesión)
6. [Recuperación de Contraseña](#6-recuperación-de-contraseña)
   - 6.1 [Solicitar Enlace de Recuperación](#61-solicitar-enlace-de-recuperación)
   - 6.2 [Restablecer Contraseña](#62-restablecer-contraseña)
7. [Interfaz Principal](#7-interfaz-principal)
   - 7.1 [Barra Superior (Header)](#71-barra-superior-header)
   - 7.2 [Barra Lateral (Sidebar)](#72-barra-lateral-sidebar)
   - 7.3 [Dashboard](#73-dashboard)
8. [Módulo de Administración](#8-módulo-de-administración)
   - 8.1 [Gestión de Usuarios](#81-gestión-de-usuarios)
   - 8.2 [Gestión de Políticas](#82-gestión-de-políticas)
9. [Tema Visual (Modo Claro / Oscuro)](#9-tema-visual-modo-claro--oscuro)
10. [Cerrar Sesión](#10-cerrar-sesión)
11. [Preguntas Frecuentes (FAQ)](#11-preguntas-frecuentes-faq)
12. [Glosario](#12-glosario)

---

## 1. Introducción

**ATLAS** (Herramienta Adaptativa para Auditoría Legislativa y Estándares) es una plataforma web integral diseñada para gestionar evaluaciones de cumplimiento normativo, seguimiento de normas y generación de reportes detallados.

### Funcionalidades principales:

| Módulo | Descripción |
|--------|-------------|
| **Gestión de Normas** | Administra y organiza normas legislativas y estándares de cumplimiento. |
| **Evaluaciones Detalladas** | Realiza evaluaciones completas de cumplimiento con seguimiento por criterio. |
| **Reportes y Análisis** | Genera reportes detallados y visualiza el progreso con gráficos interactivos. |
| **Administración RBAC** | Control de acceso basado en roles con gestión de usuarios y políticas de seguridad. |

### Roles del sistema:

| Rol | Descripción |
|-----|-------------|
| **ADMIN** | Acceso completo al sistema, incluyendo la gestión de usuarios y políticas. |
| **USER** | Acceso a las funcionalidades principales del sistema (Dashboard, Normas, Evaluaciones, Reportes). |

---

## 2. Requisitos del Sistema

Para utilizar ATLAS, necesitas:

- **Navegador web moderno** (se recomienda la última versión):
  - Google Chrome
  - Mozilla Firefox
  - Microsoft Edge
  - Safari
- **Conexión a Internet** estable.
- **Cuenta de correo electrónico** válida para el registro y la activación.

> [!NOTE]
> ATLAS es una aplicación web responsiva. Puedes acceder desde computadoras de escritorio, laptops, tablets y dispositivos móviles.

---

## 3. Acceso a la Plataforma

Accede a ATLAS a través de la URL proporcionada por tu organización.

### 3.1 Página de Inicio (Landing Page)

Al visitar la plataforma sin estar autenticado, verás la **página de inicio** con:

- **Logo y nombre** de ATLAS en la barra superior.
- **Sección Hero** con la descripción de la plataforma y botones de acción.
- **Tarjetas informativas** con las tres funcionalidades principales:
  - Gestión de Normas
  - Evaluaciones Detalladas
  - Reportes y Análisis
- **Sección CTA** con un llamado a crear tu cuenta gratuita.
- **Botones de navegación**:
  - `Iniciar Sesión` — lleva a la pantalla de login.
  - `Registrarse` — lleva al formulario de registro.
  - `Comenzar Ahora` — acceso directo al registro.

---

## 4. Registro de Usuario

### 4.1 Crear una Cuenta

1. Haz clic en **"Registrarse"** o **"Comenzar Ahora"** desde la página de inicio.
2. Completa el formulario con los siguientes datos:

| Campo | Descripción | Restricciones |
|-------|-------------|---------------|
| **Nombre** | Tu nombre real | Obligatorio, máximo 40 caracteres |
| **Apellido** | Tu apellido real | Obligatorio, máximo 40 caracteres |
| **Usuario** | Nombre de usuario único | Obligatorio, máximo 10 caracteres |
| **Correo Electrónico** | Tu correo personal o institucional | Obligatorio, formato válido, máximo 100 caracteres |

3. Haz clic en **"Registrarse"**.
4. Si el registro es exitoso, verás un mensaje de confirmación indicando que se ha enviado un correo para establecer tu contraseña.

> [!IMPORTANT]
> La contraseña **no** se define durante el registro. Se establece mediante un enlace de activación enviado a tu correo electrónico.

### 4.2 Activación de Cuenta

1. Revisa tu **bandeja de entrada** (y la carpeta de spam/no deseado) del correo electrónico que proporcionaste.
2. Abre el correo de ATLAS y haz clic en el **enlace de activación**.
3. Serás redirigido a la página de **"Establecer Contraseña"**.

### 4.3 Establecer Contraseña

En la pantalla de activación se te dará la bienvenida con tu nombre de usuario. Completa:

| Campo | Descripción | Requisitos |
|-------|-------------|------------|
| **Nueva Contraseña** | Tu contraseña de acceso | Mínimo 8 caracteres, al menos una mayúscula, una minúscula y un número |
| **Confirmar Contraseña** | Repetición de la contraseña | Debe coincidir con la contraseña anterior |

Haz clic en **"Establecer Contraseña"**. Al completarse, verás un mensaje de éxito con un enlace para **iniciar sesión**.

> [!WARNING]
> El enlace de activación tiene un **tiempo de expiración**. Si el token expira, deberás solicitar el reenvío del correo de activación.

### 4.4 Reenviar Correo de Activación

Si no recibiste el correo o el enlace expiró:

1. Después de un registro exitoso, aparecerá la opción **"Reenviar correo de activación"**.
2. Haz clic en el enlace para solicitar un nuevo correo.
3. Después de reenviar, se activa un **período de espera de 60 segundos** antes de poder solicitar otro reenvío.

---

## 5. Inicio de Sesión

1. Navega a la página de **"Iniciar Sesión"** (ruta `/login`).
2. Completa los campos:

| Campo | Descripción | Restricciones |
|-------|-------------|---------------|
| **Usuario** | Tu nombre de usuario registrado | Obligatorio, máximo 10 caracteres |
| **Contraseña** | Tu contraseña | Obligatorio |

3. Haz clic en **"Ingresar"**.
4. Si las credenciales son correctas, serás redirigido automáticamente al **Dashboard**.

> [!TIP]
> Si olvidaste tu contraseña, haz clic en **"¿Olvidaste tu contraseña?"** debajo del formulario para iniciar el proceso de recuperación.

### Errores comunes al iniciar sesión:

| Error | Causa probable | Solución |
|-------|----------------|----------|
| "Error de autenticación" | Credenciales incorrectas | Verifica tu usuario y contraseña |
| No se carga la página | Problema de conexión | Verifica tu conexión a Internet |
| Cuenta inactiva | No se completó la activación | Revisa tu correo y activa tu cuenta |

---

## 6. Recuperación de Contraseña

### 6.1 Solicitar Enlace de Recuperación

1. Desde la pantalla de login, haz clic en **"¿Olvidaste tu contraseña?"**.
2. Ingresa tu **correo electrónico** registrado.
3. Haz clic en **"Enviar Enlace"**.
4. Verás un mensaje confirmando que, si el correo está registrado, recibirás un enlace de restablecimiento.

> [!NOTE]
> Por seguridad, el sistema muestra el mismo mensaje tanto si el correo existe como si no, para prevenir la enumeración de usuarios.

### 6.2 Restablecer Contraseña

1. Abre el correo de recuperación y haz clic en el **enlace**.
2. Serás redirigido a la pantalla de **"Restablecer Contraseña"**.
3. Ingresa tu nueva contraseña:

| Campo | Requisitos |
|-------|------------|
| **Nueva Contraseña** | Mínimo 8 caracteres, una mayúscula, una minúscula y un número |
| **Confirmar Contraseña** | Debe coincidir exactamente |

4. Haz clic en **"Restablecer Contraseña"**.
5. Tras el éxito, podrás iniciar sesión con tu nueva contraseña.

---

## 7. Interfaz Principal

Una vez autenticado, accederás a la interfaz principal de ATLAS, compuesta por tres áreas:

```
┌─────────────────────────────────────────────────┐
│              BARRA SUPERIOR (Header)            │
├──────────┬──────────────────────────────────────┤
│          │                                      │
│  BARRA   │                                      │
│ LATERAL  │        ÁREA DE CONTENIDO             │
│(Sidebar) │           (Dashboard)                │
│          │                                      │
│          │                                      │
└──────────┴──────────────────────────────────────┘
```

### 7.1 Barra Superior (Header)

La barra superior contiene los siguientes elementos:

| Elemento | Ubicación | Función |
|----------|-----------|---------|
| **☰ (Menú hamburguesa)** | Izquierda | Muestra/oculta la barra lateral |
| **Logo ATLAS** | Izquierda | Enlace al Dashboard |
| **Badge de Rol** | Derecha | Muestra tu rol actual (ADMIN / USER) |
| **Nombre de usuario** | Derecha | Identifica tu sesión activa |
| **☀ / 🌙 (Tema)** | Derecha | Alterna entre modo claro y oscuro |
| **Salir** | Derecha | Cierra tu sesión |

### 7.2 Barra Lateral (Sidebar)

La barra lateral contiene la navegación principal del sistema:

**Sección "Principal":**

| Opción | Icono | Estado |
|--------|-------|--------|
| Dashboard | 📊 | Disponible |
| Normas | 📄 | *Próximamente* |
| Evaluaciones | ✅ | *Próximamente* |
| Reportes | 📈 | *Próximamente* |

**Sección "Administración"** *(visible solo para rol ADMIN)*:

| Opción | Icono | Estado |
|--------|-------|--------|
| Usuarios | 👥 | Disponible |
| Políticas | 🛡️ | Disponible |

> [!NOTE]
> Los módulos marcados como *"Próximamente"* aparecen deshabilitados y se activarán en futuras versiones.

### 7.3 Dashboard

El **Dashboard** es la página principal tras iniciar sesión. Muestra:

- **Saludo personalizado**: "Bienvenido, [tu nombre de usuario]".
- **Tarjetas de acceso rápido** *(solo para administradores)*:
  - **Gestión de Usuarios** — acceso directo al módulo de administración de usuarios.
  - **Gestión de Políticas** — acceso directo al módulo de administración de políticas.

---

## 8. Módulo de Administración

> [!IMPORTANT]
> Las funciones de administración están disponibles **únicamente para usuarios con rol ADMIN**.

### 8.1 Gestión de Usuarios

**Ruta:** `/admin/usuarios`

Este módulo permite administrar todos los usuarios del sistema.

#### Listado de Usuarios

Al acceder, se muestra una cuadrícula de tarjetas de usuario, cada una con:

- **Avatar** e icono de usuario.
- **Nombre completo** y **nombre de usuario** (precedido de @).
- **Rol** del usuario (badge).
- **Correo electrónico**.
- **Fecha de creación**.
- **Botones de acción**:
  - `Editar` — modifica los datos del usuario.
  - `Eliminar` — elimina el usuario con confirmación.
  - `Políticas` — asigna políticas de seguridad al usuario.

> [!CAUTION]
> Los usuarios con rol **ADMIN** del sistema no pueden ser editados ni eliminados para proteger la integridad del sistema.

#### Crear Usuario

1. Haz clic en el botón **"Crear Usuario"** (esquina superior derecha).
2. Se abrirá un modal con el formulario:

| Campo | Descripción | Restricciones |
|-------|-------------|---------------|
| **Nombre de Usuario** | Identificador único | Obligatorio, máx. 10 caracteres |
| **Correo** | Correo electrónico | Obligatorio, formato válido |
| **Nombre** | Nombre del usuario | Obligatorio, máx. 40 caracteres |
| **Apellido** | Apellido del usuario | Obligatorio, máx. 40 caracteres |
| **Rol** | Rol asignado | Selección obligatoria |
| **Contraseña** | Contraseña inicial | Obligatoria al crear |

3. Haz clic en **"Guardar"** para crear el usuario.

#### Editar Usuario

1. En la tarjeta del usuario, haz clic en **"Editar"**.
2. Modifica los campos deseados en el modal.
3. El campo de contraseña es **opcional** al editar (déjalo vacío para mantener la contraseña actual).
4. Haz clic en **"Guardar"** para aplicar los cambios.

#### Eliminar Usuario

1. En la tarjeta del usuario, haz clic en **"Eliminar"**.
2. Aparecerá un diálogo de confirmación:
   > *"¿Estás seguro de que deseas eliminar al usuario **[Nombre Completo]**? Esta acción no se puede deshacer."*
3. Haz clic en **"Eliminar"** para confirmar o **"Cancelar"** para abortar.

#### Asignar Políticas a un Usuario

1. En la tarjeta del usuario, haz clic en **"Políticas"**.
2. Se abrirá un modal con las políticas disponibles.
3. Selecciona las políticas que deseas asignar.
4. Haz clic en **"Guardar"** para aplicar las asignaciones.

---

### 8.2 Gestión de Políticas

**Ruta:** `/admin/politicas`

Este módulo permite administrar las **políticas de seguridad** del sistema y su asignación a roles.

#### Flujo de Trabajo

```
┌───────────────────┐     ┌──────────────────────┐     ┌──────────────────────┐
│  1. Seleccionar   │────▶│  2. Ver políticas     │────▶│  3. Asignar /        │
│     un Rol        │     │     asignadas         │     │     Desasignar       │
└───────────────────┘     └──────────────────────┘     └──────────────────────┘
```

#### Paso 1: Seleccionar un Rol

- En la parte superior se muestran los **roles disponibles** como botones.
- Haz clic en un rol para ver sus políticas asociadas.
- El rol seleccionado se resaltará visualmente.

#### Paso 2: Ver Políticas del Rol

Una vez seleccionado un rol, se muestran dos secciones:

**Políticas Asignadas** (marca verde ✅):
- Lista de políticas actualmente vinculadas al rol.
- Cada política muestra su nombre y un badge "Asignada".
- Incluye el botón **"Desasignar"** para remover la política del rol.

**Políticas Disponibles** (sin asignar):
- Lista de políticas que aún no están vinculadas al rol.
- Cada política muestra su nombre y un badge "No asignada".
- Incluye el botón **"Asignar"** para vincular la política al rol.

#### Paso 3: Asignar / Desasignar Políticas

| Acción | Botón | Efecto |
|--------|-------|--------|
| **Asignar** | `+ Asignar` (botón primario) | Vincula la política al rol seleccionado |
| **Desasignar** | `✕ Desasignar` (botón rojo) | Remueve la política del rol seleccionado |

> [!TIP]
> Las acciones de asignar y desasignar se ejecutan de forma individual. El sistema muestra un indicador de carga en el botón mientras procesa la operación.

---

## 9. Tema Visual (Modo Claro / Oscuro)

ATLAS soporta dos modos de visualización:

| Modo | Descripción |
|------|-------------|
| ☀️ **Claro** | Fondo claro con texto oscuro. Ideal para ambientes con mucha luz. |
| 🌙 **Oscuro** | Fondo oscuro con texto claro. Reduce la fatiga visual en ambientes con poca luz. |

**Para cambiar el tema:**
1. Haz clic en el ícono de **sol** (☀️) o **luna** (🌙) en la barra superior.
2. El cambio se aplica instantáneamente en toda la interfaz.
3. Tu preferencia se guarda automáticamente para futuras sesiones.

---

## 10. Cerrar Sesión

Para cerrar tu sesión de forma segura:

1. Haz clic en el botón **"Salir"** ubicado en la esquina superior derecha de la barra superior.
2. Tu sesión se cerrará y serás redirigido a la página de **inicio de sesión**.

> [!IMPORTANT]
> Al cerrar sesión, tu token de autenticación se elimina del navegador. Necesitarás ingresar tus credenciales nuevamente para acceder al sistema.

---

## 11. Preguntas Frecuentes (FAQ)

### ¿Qué hago si no recibo el correo de activación?

1. Revisa tu carpeta de **spam** o **correo no deseado**.
2. Verifica que ingresaste correctamente tu correo electrónico durante el registro.
3. Utiliza la opción **"Reenviar correo de activación"** que aparece después del registro.
4. Si el problema persiste, contacta al administrador del sistema.

### ¿Mi enlace de activación expiró, qué hago?

Solicita un nuevo enlace utilizando la opción de **"Reenviar correo de activación"** o contacta al administrador del sistema para que te genere uno nuevo.

### ¿Cuáles son los requisitos para la contraseña?

Tu contraseña debe cumplir con **todos** los siguientes requisitos:
- Mínimo **8 caracteres**.
- Al menos **una letra mayúscula** (A-Z).
- Al menos **una letra minúscula** (a-z).
- Al menos **un número** (0-9).

### ¿Cómo sé qué rol tengo?

Tu rol se muestra como un **badge** (etiqueta) junto a tu nombre de usuario en la barra superior del sistema.

### ¿Por qué algunas opciones del menú dicen "Próximamente"?

Los módulos de **Normas**, **Evaluaciones** y **Reportes** están planificados para futuras versiones de la plataforma. Aparecen deshabilitados en el menú lateral como referencia.

### ¿Puedo usar ATLAS en mi celular?

Sí. ATLAS está diseñada como una aplicación web **responsiva**, lo que significa que se adapta al tamaño de la pantalla de tu dispositivo. Puedes acceder desde cualquier navegador móvil moderno.

### ¿Es seguro el sistema?

Sí. ATLAS implementa las siguientes medidas de seguridad:
- Autenticación mediante **tokens JWT** con expiración automática.
- Contraseñas cifradas con **BCrypt**.
- Control de acceso basado en **roles y políticas (RBAC)**.
- Protección contra **enumeración de usuarios** en los flujos de recuperación.
- Comunicación cifrada mediante **HTTPS**.

---

## 12. Glosario

| Término | Definición |
|---------|------------|
| **ATLAS** | Herramienta Adaptativa para Auditoría Legislativa y Estándares. |
| **RBAC** | Control de Acceso Basado en Roles (*Role-Based Access Control*). |
| **JWT** | JSON Web Token — estándar de autenticación basado en tokens. |
| **Política** | Permiso o regla de seguridad que define qué acciones puede realizar un rol o usuario. |
| **Rol** | Clasificación de un usuario que determina su nivel de acceso (ej. ADMIN, USER). |
| **Token de activación** | Código único y temporal enviado por correo para verificar y activar una cuenta. |
| **Dashboard** | Panel de control principal que muestra un resumen y accesos directos a las funciones del sistema. |
| **Modo oscuro** | Tema visual con fondo oscuro que reduce la emisión de luz de la pantalla. |

---

<p align="center">
  <strong>© 2026 ATLAS</strong> — Herramienta Adaptativa para Auditoría Legislativa y Estándares<br>
  <em>Todos los derechos reservados.</em>
</p>
