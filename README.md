<div align="center">

<img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/assets/banner.svg" width="100%" alt="Rubén Juan Candela — Full Stack Developer" />

</div>

## Sobre mí

Graduado en **DAM** con experiencia real en sistemas en producción, no solo en proyectos de clase.

He construido y desplegado un backend Spring Boot con su app Android, un bot de Discord de ~27k líneas de Java, y un sistema interno en producción para una cooperativa energética real (**Enercoop**) — con ownership completo en todos: base de datos, backend, frontend, despliegue y documentación.

En **octubre de 2026** empiezo el curso de especialización en **IA y Big Data** (600 h, IES Severo Ochoa, Elche), y mientras tanto me estoy preparando por mi cuenta con un plan estructurado de 16 semanas.

> 🟢 **Abierto a nuevas oportunidades** como Full Stack / Backend Java / Frontend React.

---

## Proyecto destacado

### 🤖 GymProBot — Bot de Discord con economía RPG y API propia

> Comunidad fitness gamificada sobre Discord, conectada en vivo con la API de GymProFit

<p>
<img src="https://img.shields.io/badge/Java%2021-21262D?style=flat-square" alt="Java 21">
<img src="https://img.shields.io/badge/JDA%205-21262D?style=flat-square" alt="JDA 5">
<img src="https://img.shields.io/badge/Retrofit2%20%2B%20OkHttp-21262D?style=flat-square" alt="Retrofit2 + OkHttp">
<img src="https://img.shields.io/badge/Aiven%20MySQL-21262D?style=flat-square" alt="Aiven MySQL">
<img src="https://img.shields.io/badge/Flyway-21262D?style=flat-square" alt="Flyway">
<img src="https://img.shields.io/badge/HikariCP-21262D?style=flat-square" alt="HikariCP">
<img src="https://img.shields.io/badge/Docker-21262D?style=flat-square" alt="Docker">
<img src="https://img.shields.io/badge/Render-21262D?style=flat-square" alt="Render">
<img src="https://img.shields.io/badge/GitHub%20Actions-21262D?style=flat-square" alt="GitHub Actions">
</p>

| **253** | **~26.600** | **+60** | **556** |
|:--:|:--:|:--:|:--:|
| clases Java | líneas de Java | comandos slash | tests |

- **Arquitectura por capas propia, sin framework:** `commands` · `services` · `api` · `db` · `embeds` · `jobs` · `i18n`
- **Economía RPG completa:** progresión y XP, trabajo y carrera, empresas con gobernanza e impuestos, combate por turnos, minería y crafteo, banca, bolsa, gremios y mercado entre jugadores
- **32 migraciones Flyway** sobre 35 tablas · tests con JUnit 5, Mockito, MockWebServer y Testcontainers como gate de CI
- **Bilingüe ES/EN** con `ResourceBundle`, jobs programados con TZ fija y health server sin Spring (`com.sun.net.httpserver`)
- **RGPD por diseño:** texto libre cifrado con AES-256-GCM, comandos de exportación y borrado de datos, y job de retención automática
- **Docker multi-stage** desplegado en Render con blueprint (`render.yaml`), health check y secretos fuera del repo

<a href="https://github.com/ruubeenn13/gymprofit-bot">Ver repositorio →</a>

---

## Más proyectos

<table>
<tr>
<td width="50%" valign="top">

### 💪 GymProFit

<em>App Android + API REST en producción · TFG</em>

<p>
<img src="https://img.shields.io/badge/Java%2021-21262D?style=flat-square" alt="Java 21">
<img src="https://img.shields.io/badge/Spring%20Boot%203-21262D?style=flat-square" alt="Spring Boot 3">
<img src="https://img.shields.io/badge/MariaDB%20%2F%20MySQL-21262D?style=flat-square" alt="MariaDB / MySQL">
<img src="https://img.shields.io/badge/jOOQ-21262D?style=flat-square" alt="jOOQ">
<img src="https://img.shields.io/badge/MapStruct-21262D?style=flat-square" alt="MapStruct">
<img src="https://img.shields.io/badge/JWT-21262D?style=flat-square" alt="JWT">
<img src="https://img.shields.io/badge/AWS%20EC2-21262D?style=flat-square" alt="AWS EC2">
<img src="https://img.shields.io/badge/nginx-21262D?style=flat-square" alt="nginx">
</p>

<ul>
<li>API REST en <b>Spring Boot 3 + Java 21</b>, con jOOQ para consultas tipadas y MapStruct para el mapeo de DTOs</li>
<li>Base de datos de <b>18 tablas</b> con migraciones versionadas en Flyway</li>
<li>App <b>Android en Java</b>: autenticación JWT, modo invitado y multiidioma (ES/EN)</li>
<li><b>Desplegada en dos infraestructuras reales:</b> AWS EC2 con nginx como reverse proxy y servicio systemd con reinicio automático, y Render + Aiven MySQL con TLS <code>verify-full</code></li>
</ul>

<a href="https://github.com/ruubeenn13/TFG-GymProFit">Ver repositorio →</a>

</td>
<td width="50%" valign="top">

### 🎫 Gestor de Turnos — Enercoop

<em>Cola de atención presencial para una cooperativa energética · En producción</em>

<p>
<img src="https://img.shields.io/badge/React%2019-21262D?style=flat-square" alt="React 19">
<img src="https://img.shields.io/badge/Vite-21262D?style=flat-square" alt="Vite">
<img src="https://img.shields.io/badge/Supabase-21262D?style=flat-square" alt="Supabase">
<img src="https://img.shields.io/badge/PostgreSQL-21262D?style=flat-square" alt="PostgreSQL">
<img src="https://img.shields.io/badge/Docker%20Compose-21262D?style=flat-square" alt="Docker Compose">
<img src="https://img.shields.io/badge/Vitest-21262D?style=flat-square" alt="Vitest">
<img src="https://img.shields.io/badge/GitLab%20CI%2FCD-21262D?style=flat-square" alt="GitLab CI/CD">
</p>

<ul>
<li><b>Supabase autoalojado</b> con Docker Compose (13 contenedores): auth, API REST, Edge Functions y lógica de negocio</li>
<li>PostgreSQL con esquema relacional, <b>RLS por roles</b> y RPCs</li>
<li>Frontend React + Vite con actualizaciones <b>en tiempo real</b> vía Supabase Realtime</li>
<li><b>5 perfiles de usuario</b> (admin, gestor, usuario, kiosko, display), reasignación automática y módulo de estadísticas</li>
<li>Multiidioma <b>ES/VAL/EN</b> · agente de kiosko independiente · pipeline de CI/CD en GitLab</li>
</ul>

<em>Proyecto interno en producción — repositorio privado</em>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧠 iabd-prep

<em>Plan de autoformación de 16 semanas en IA y Big Data</em>

<p>
<img src="https://img.shields.io/badge/Python-21262D?style=flat-square" alt="Python">
<img src="https://img.shields.io/badge/MongoDB-21262D?style=flat-square" alt="MongoDB">
<img src="https://img.shields.io/badge/AWS-21262D?style=flat-square" alt="AWS">
<img src="https://img.shields.io/badge/Hadoop-21262D?style=flat-square" alt="Hadoop">
<img src="https://img.shields.io/badge/Spark-21262D?style=flat-square" alt="Spark">
<img src="https://img.shields.io/badge/Kafka-21262D?style=flat-square" alt="Kafka">
<img src="https://img.shields.io/badge/Airflow-21262D?style=flat-square" alt="Airflow">
</p>

<ul>
<li>Ruta estructurada: Python base → NoSQL → Cloud → Big Data/ETL → Hadoop → Spark → Kafka/NiFi/Airflow → Hugging Face → IoT</li>
<li>Ejercicios y notebooks propios, con progreso semanal versionado</li>
<li>Preparación para el curso de especialización que empiezo en octubre</li>
</ul>

<a href="https://github.com/ruubeenn13/iabd-prep">Ver repositorio →</a>

</td>
<td width="50%" valign="top">

### 📁 Anteriores

<em>Primeros proyectos del ciclo</em>

<p>
<img src="https://img.shields.io/badge/Android-21262D?style=flat-square" alt="Android">
<img src="https://img.shields.io/badge/SQLite-21262D?style=flat-square" alt="SQLite">
<img src="https://img.shields.io/badge/JavaScript-21262D?style=flat-square" alt="JavaScript">
<img src="https://img.shields.io/badge/HTML%20%2F%20CSS-21262D?style=flat-square" alt="HTML / CSS">
</p>

<ul>
<li><b><a href="https://lamarmitaparallevar.com">La Marmita Para Llevar</a></b> — web corporativa para restaurante de comida para llevar: menú, pedidos, horarios y FAQ. Responsive y desplegada con dominio propio.</li>
<li><b><a href="https://github.com/ruubeenn13/filmoteca-RubenJuan">Filmoteca</a></b> — app Android de gestión de colecciones de películas: autenticación, CRUD completo, reproducción multimedia y notificaciones locales.</li>
</ul>

</td>
</tr>
</table>

---

## Stack

| Área | Tecnologías |
|------|-------------|
| **Backend** | Java 21 · Spring Boot 3 · JDA 5 · Python · APIs REST |
| **Frontend** | React 19 · Vite · JavaScript · HTML · CSS |
| **Bases de datos** | PostgreSQL · MySQL · MariaDB · SQLite · Supabase |
| **Persistencia** | Flyway · jOOQ · MapStruct · HikariCP · JDBC |
| **Cloud & Infra** | AWS EC2 · Render · Aiven · Docker · nginx · systemd |
| **CI/CD & Testing** | GitHub Actions · GitLab CI/CD · JUnit 5 · Mockito · Testcontainers · Vitest |
| **Mobile** | Android (Java) |
| **Otros** | JWT · Retrofit2 · OkHttp · Swagger/OpenAPI · Git · i18n (ES/VAL/EN) |

---

## Formación

| | |
|---|---|
| **Especialización en IA y Big Data** · 600 h *(desde oct. 2026)* | IES Severo Ochoa, Elche |
| **CFGS DAM** — Desarrollo de Aplicaciones Multiplataforma | IES Macià Abela, Crevillente · 2024–2026 |
| **CFGM SMR** — Sistemas Microinformáticos y Redes | IES Macià Abela, Crevillente · 2022–2024 |

---

## Actividad

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/output/github-snake.svg" />
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/output/github-snake.svg" width="100%" alt="Gráfico de contribuciones" />
</picture>

<br/><br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/0-profile-details.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github/0-profile-details.svg" />
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/0-profile-details.svg" width="90%" alt="Resumen del perfil" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/3-stats.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github/3-stats.svg" />
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/3-stats.svg" width="49%" alt="Estadísticas" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/4-productive-time.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github/4-productive-time.svg" />
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/4-productive-time.svg" width="49%" alt="Horario productivo" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/1-repos-per-language.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github/1-repos-per-language.svg" />
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/1-repos-per-language.svg" width="49%" alt="Repositorios por lenguaje" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/2-most-commit-language.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github/2-most-commit-language.svg" />
  <img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/2-most-commit-language.svg" width="49%" alt="Lenguajes más usados" />
</picture>

</div>

---

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rubén_Juan_Candela-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rub%C3%A9n-juan-candela-9743a026a)
[![Email](https://img.shields.io/badge/rubenjuancandela06@gmail.com-E8710A?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rubenjuancandela06@gmail.com)

</div>
