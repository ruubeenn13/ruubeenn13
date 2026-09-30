<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/banner-light.svg">
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/banner-light.svg" width="100%" alt="Rubén Juan Candela · Full Stack Developer · Java, Spring Boot, React y TypeScript. Disponible. De la base de datos al despliegue, sin saltarse ninguna capa.">
</picture>

🟢 **Disponible · incorporación inmediata** — Full Stack, Backend Java o Frontend React<br>
📍 Alicante · Elche · remoto &nbsp;·&nbsp; Español nativo · Inglés B2

<a href="https://www.linkedin.com/in/rubenjuancandela"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/contacto-linkedin-dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/contacto-linkedin-light.svg"><img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/contacto-linkedin-light.svg" height="40" alt="LinkedIn"></picture></a>
<a href="mailto:rubenjuancandela06@gmail.com"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/contacto-email-dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/contacto-email-light.svg"><img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/contacto-email-light.svg" height="40" alt="Email: rubenjuancandela06@gmail.com"></picture></a>

</div>

**Desarrollador Full Stack junior** (DAM, 2026). Me ocupo de todas las capas: modelo de datos, API, frontend, tests y despliegue.

En **Grupo Enercoop** diseñé y construí desde cero un gestor de turnos en tiempo real que hoy está **en producción**. Por mi cuenta mantengo **GymProFit** (API Spring Boot + app Android + panel React) y **GymProBot**, un bot de Discord que se prueba y se despliega solo en mi propio servidor Linux.

<sub>*EN: Junior full-stack developer who builds, tests and ships — from the database to deployment.*</sub>

## Lo que he construido

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/proyecto-enercoop-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/proyecto-enercoop-light.svg">
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/proyecto-enercoop-light.svg" width="100%" alt="Gestor de turnos en tiempo real para Grupo Enercoop, en producción: 139 tests con Vitest, 13 contenedores Docker y seguridad por roles con RLS. Panel React + Vite, Supabase autoalojado con PostgreSQL detrás de nginx y agente Python para kiosko y puestos con escáner e impresora térmica.">
</picture>

- **Lógica en PostgreSQL:** asignación automática de turnos por prioridad y seguridad por roles con **RLS**.
- **Supabase autoalojado** en Docker (13 contenedores) detrás de nginx, con **CI/CD en GitLab** y **139 tests** automatizados con Vitest.
- **Agente en Python** para los puestos de atención y el kiosko, integrado con escáner e impresora térmica.

<sub>Prácticas FCT (400 h, mar–jun 2026) y después contrato temporal (jun–jul 2026) para desplegarlo. Sistema interno de la empresa: sin enlace ni capturas.</sub>

<br>

<a href="https://github.com/ruubeenn13/GymProFit">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/proyecto-gymprofit-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/proyecto-gymprofit-light.svg">
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/proyecto-gymprofit-light.svg" width="100%" alt="GymProFit: app Android, API REST en Spring Boot con JWT, refresh token rotado y roles, y panel web en React + TypeScript. Más de 870 tests en CI, 239 endpoints REST y 25 tablas en MySQL. API en api.gymprofit.app.">
</picture>
</a>

- **Spring Security con JWT**, refresh token rotado y permisos por rol (`ADMIN`, `USER`, `GUEST`).
- **Audité mi propia API:** encontré y cerré varias vulnerabilidades IDOR y una escalada de privilegios, y cubrí con tests de acceso ajeno las rutas con id.
- **CI en GitHub Actions** para la API (contra una MariaDB efímera), la app Android y el panel web; las actualizaciones de Dependabot solo se fusionan con el CI en verde.
- API desplegada primero en **AWS EC2** y después en **Render**, con dominio propio (`api.gymprofit.app`); el panel vive en `admin.gymprofit.app`, detrás de Cloudflare Access.

**[Ver el repositorio de GymProFit →](https://github.com/ruubeenn13/GymProFit)**

<br>

<a href="https://github.com/ruubeenn13/gymprofit-bot">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/proyecto-gymprobot-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/proyecto-gymprobot-light.svg">
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/proyecto-gymprobot-light.svg" width="100%" alt="GymProBot: bot de Discord en Java 21 + JDA 5 conectado a la API de GymProFit. 65 comandos slash, más de 660 tests y unas 21 000 líneas de Java. Cada push a main pasa el CI y, solo si está en verde, se construye la imagen Docker y se despliega en el homelab con aviso por ntfy.">
</picture>
</a>

- **Sin framework:** arquitectura por capas propia sobre JDA, sin Spring (comandos, servicios, cliente de API, repositorios JDBC, jobs e i18n ES/EN).
- **Despliegue continuo:** cada push a `main` pasa build y tests (JUnit 5, Mockito y Testcontainers con MySQL real); solo si el CI está en verde, un runner self-hosted construye la imagen Docker y la despliega en mi homelab, con aviso por ntfy.
- **Cliente de la API de GymProFit** con Retrofit: JWT con renovación ante 401, caché y reintentos con backoff.
- **RGPD por diseño:** texto libre cifrado con AES-256-GCM, exportación y borrado de datos y retención automática. 39 migraciones Flyway sobre 38 tablas.

**[Ver el repositorio de GymProBot →](https://github.com/ruubeenn13/gymprofit-bot)**

### También

- **[Homelab](https://github.com/ruubeenn13/homelab)** — Portátil reutilizado con Ubuntu Server 24.04 y Docker Compose: 14 stacks, Traefik v3 con TLS wildcard, Prometheus + Grafana, Uptime Kuma + ntfy, backups 3-2-1 (restic + Backblaze B2) y ningún puerto abierto al exterior (Cloudflare Tunnel + Tailscale). Aquí vive GymProBot.

## Stack

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/stack-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/stack-light.svg">
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/stack-light.svg" width="100%" alt="Stack. Backend: Java, Spring Boot, Spring Security, Python, Maven, JUnit 5 y Flyway. Frontend y móvil: React, TypeScript, JavaScript, Vite, Vitest, Android, HTML5 y CSS3. DevOps y datos: Docker, Linux, nginx, Traefik, GitHub Actions, GitLab CI/CD, Cloudflare, AWS, PostgreSQL, MySQL, Supabase, Prometheus y Grafana.">
</picture>

## Ahora mismo

- Desde **octubre de 2026** curso la **Especialización en Inteligencia Artificial y Big Data** (IES Severo Ochoa, Elche · 600 h · lunes, miércoles y viernes de 17 a 21 h).
- Preparación por mi cuenta en Python, pandas, MongoDB y AWS: [iabd-prep](https://github.com/ruubeenn13/iabd-prep).

## Formación

| Título | Centro | Años |
|---|---|---|
| **CFGS Desarrollo de Aplicaciones Multiplataforma (DAM)** | IES Macià Abela, Crevillente | 2024–2026 |
| **CFGM Sistemas Microinformáticos y Redes (SMR)** | IES Macià Abela, Crevillente | 2022–2024 |

## Contacto

¿Tienes un puesto **Full Stack, Backend Java o Frontend React** en Alicante, Elche o en remoto? Escríbeme a **rubenjuancandela06@gmail.com** o por **[LinkedIn](https://www.linkedin.com/in/rubenjuancandela)**.
