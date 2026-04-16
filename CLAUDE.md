# CLAUDE.md — Mapa de Navegación del Sistema
> Generado automáticamente el 2026-04-16. Actualizar cuando cambie la infraestructura.

---

## 1. Identidad y Ubicación

| Campo | Valor |
|---|---|
| **Usuario del sistema** | `claudecode01` (uid=1001) |
| **Grupos** | `claudecode01`, `sudo`, `docker` |
| **Proyecto activo** | `/home/claudecode01/mi-proyecto` |
| **Repositorio GitHub** | `PonchoXp360/mi-proyecto` |
| **Git user** | PonchoXp360 / poncho.xp.360@gmail.com |
| **Rama principal** | `master` |

**Archivos en este proyecto:**
- `README.md` — vacío (pendiente de completar)
- `prueba_final.py` — script de prueba: `print("Todo funciona perfecto, Poncho")`

---

## 2. Infraestructura del Servidor

### Sistema Operativo
- **OS:** Ubuntu 24.04.4 LTS (Noble Numbat)
- **Kernel:** Linux 6.8.0-107-generic x86_64
- **Hostname:** srv1535743

### Hardware
| Recurso | Detalle |
|---|---|
| **CPU** | AMD EPYC 9354P 32-Core (2 vCPUs asignados) |
| **RAM total** | 7.8 GiB |
| **RAM disponible** | ~4.7 GiB |
| **Swap** | 4.0 GiB (2.0 GiB en uso) |
| **Disco** | 96 GB total · 58 GB usados (61%) · 39 GB libres |

### Red
| Interfaz | IP |
|---|---|
| **IP pública** | `187.77.14.222` |
| **IPv6** | `2a02:4780:2d:668f::1` |
| **localhost** | `127.0.0.1` |
| **Docker bridge** | `10.0.0.0/24` + redes `10.0.1-8.x` |

---

## 3. Herramientas de Desarrollo Instaladas

| Herramienta | Versión |
|---|---|
| **Node.js** | v18.19.1 |
| **npm** | 9.2.0 |
| **Python** | 3.12.3 |
| **Git** | 2.43.0 |
| **Docker** | 29.4.0 |
| **curl** | 8.5.0 |
| pnpm | no instalado |
| bun | no instalado |
| gh CLI | no instalado |

---

## 4. Conectividad con GitHub

- **Estado SSH:** AUTENTICADO (`Hi PonchoXp360! You've successfully authenticated`)
- **Llave SSH:** ED25519 en `~/.ssh/id_ed25519`
  - Clave pública: `ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIAN8KC4fMHC/qYYFVCCHHElRZ5era4Jcubp15erZ5dHd`
- **Remote origin:** `git@github.com:PonchoXp360/mi-proyecto.git`
- **Known hosts:** github.com verificado

---

## 5. Proyectos en el Sistema

### `/home/claudecode01/mi-proyecto` ← (este repo)
Proyecto de arranque / pruebas con Python. Repositorio limpio.

### `/home/claudecode01/Tienda-virtual`
E-commerce completo con stack moderno:
- **Framework:** Next.js (TypeScript) + Tailwind CSS
- **ORM:** Prisma
- **Auth:** better-auth
- **Deploy:** Firebase App Hosting (`apphosting.yaml`)
- **Config extra:** `components.json`, `middleware.ts`

### `/home/claudecode01/projects`
Workspace de infraestructura / DevOps. Contiene:
- `scripts/` — health checks y automatizaciones
- `docs/`, `logs/`, `configs/`, `backups/`
- Carpetas por servicio: `n8n/`, `wordpress/`, `odoo/`, `nextcloud/`, `openclaw/`
- Su propio `CLAUDE.md` con contexto de infraestructura

---

## 6. Servicios y Contenedores Activos

El servidor corre múltiples servicios Docker con **Traefik** como reverse proxy (API en `localhost:8080`).

| Servicio | Dominio |
|---|---|
| **Sitio principal** | rpyasociados.com / rpyasociados.tech |
| **WordPress** | wordpress.rpyasociados.tech |
| **n8n** (automatización) | n8n.rpyasociados.tech |
| **Nextcloud** | subdominio sslip.io |
| **Odoo** | subdominio sslip.io |
| **Openclaw** | subdominio sslip.io |
| **Coolify** | coolify.rpyasociados.tech |
| **Traefik** | localhost:8080 (panel interno) |

---

## 7. Integraciones Activas

### Antigravity (VS Code Remote Server)
- **Ubicación:** `~/.antigravity-server/`
- **Versión:** 1.22.2 (commit `62335c71`)
- **Estado:** ACTIVO — Language Server iniciado y corriendo
- **Función:** Servidor remoto de VS Code (permite editar este servidor desde VS Code desktop via Remote SSH o similar)
- **Log relevante:** `(Antigravity) Language server started` — `LS lspClient started successfully`

### Gemini
- **Config:** `~/.gemini/antigravity/`
- **Estado:** Configurado (integración con Google Gemini AI)

### Claude Code
- **Config global:** `~/.claude/settings.local.json`
- **Permisos:** Extenso set de permisos pre-autorizados (Bash, Docker, git, npm, curl, etc.)
- **Memoria persistente:** `~/.claude/projects/`

---

## 8. Cómo Trabajamos Juntos

### Flujo de trabajo estándar
1. Siempre verificar rama activa con `git status` antes de hacer cambios
2. Commits pequeños y descriptivos en inglés o español (consistente con el repo)
3. Push a `origin/master` solo cuando el trabajo esté probado

### Reglas de este proyecto
- Este proyecto es para pruebas y aprendizaje — no hay restricciones de stack
- El archivo `prueba_final.py` valida que el entorno Python funciona
- `README.md` está vacío — completar cuando el proyecto tenga un propósito definido

### Para tareas de infraestructura
Trabajar desde `/home/claudecode01/projects` — tiene su propio `CLAUDE.md` con contexto específico de los servicios Docker y dominios.

### Para la Tienda Virtual
Trabajar desde `/home/claudecode01/Tienda-virtual` — proyecto Next.js con su propio `CLAUDE.md`.
