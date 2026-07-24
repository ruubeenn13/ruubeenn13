<div align="center">

```
██████╗ ██╗   ██╗██████╗ ███████╗███╗   ██╗
██╔══██╗██║   ██║██╔══██╗██╔════╝████╗  ██║
██████╔╝██║   ██║██████╔╝█████╗  ██╔██╗ ██║
██╔══██╗██║   ██║██╔══██╗██╔══╝  ██║╚██╗██║
██║  ██║╚██████╔╝██████╔╝███████╗██║ ╚████║
╚═╝  ╚═╝ ╚═════╝ ╚═════╝ ╚══════╝╚═╝  ╚═══╝
```

### Full Stack Developer · Crevillente, Alicante 🇪🇸

*Backend en Java, frontend en React y todo lo que hace falta para que llegue a producción*

<br/>

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL_·_MariaDB-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

</div>

---

## Sobre mí

Graduado en **DAM** con experiencia real en sistemas en producción, no solo en proyectos de clase.

He construido y desplegado un backend Spring Boot con su app Android, un bot de Discord de ~27k líneas de Java, y un sistema interno en producción para una cooperativa energética real (**Enercoop**) — con ownership completo en todos: base de datos, backend, frontend, despliegue y documentación.

En **octubre de 2026** empiezo el curso de especialización en **IA y Big Data** (600 h, IES Severo Ochoa, Elche), y mientras tanto me estoy preparando por mi cuenta con un plan estructurado de 16 semanas.

> 🟢 **Abierto a nuevas oportunidades** como Full Stack / Backend Java / Frontend React.

---

## 🏗️ Proyectos

### 🤖 GymProBot — Bot de Discord con economía RPG y API propia
> Comunidad fitness gamificada sobre Discord, conectada en vivo con la API de GymProFit

**Stack:** `Java 21` `JDA 5` `Retrofit2 + OkHttp` `Aiven MySQL` `Flyway` `HikariCP` `Docker` `Render` `GitHub Actions`

- **253 clases · ~26.600 líneas de Java** sin framework: arquitectura por capas propia (`commands` · `services` · `api` · `db` · `embeds` · `jobs` · `i18n`)
- **+60 comandos slash**: progresión y XP, economía, combate por turnos, minería y crafteo, empresas con gobernanza e impuestos, banca, bolsa, gremios y mercado entre jugadores
- **32 migraciones Flyway** sobre 35 tablas · **556 tests** (JUnit 5, Mockito, MockWebServer, Testcontainers) como gate de CI
- **Bilingüe ES/EN** con `ResourceBundle`, jobs programados con TZ fija y health server sin Spring (`com.sun.net.httpserver`)
- **RGPD por diseño:** texto libre cifrado con AES-256-GCM, comandos de exportación y borrado de datos, y job de retención automática
- Despliegue **Docker multi-stage** en Render con blueprint (`render.yaml`), health check y secretos fuera del repo

🔗 [Ver repositorio](https://github.com/ruubeenn13/gymprofit-bot)

---

### 💪 GymProFit — App Android + API REST en producción
> App de fitness y nutrición con backend propio · Proyecto de fin de grado (TFG)

**Stack:** `Java 21` `Spring Boot 3` `MariaDB / MySQL` `Flyway` `jOOQ` `MapStruct` `JWT` `AWS EC2` `nginx` `Render` `Aiven`

- API REST en **Spring Boot 3 + Java 21**, con jOOQ para consultas tipadas y MapStruct para el mapeo de DTOs
- Base de datos de **18 tablas** con migraciones versionadas en Flyway
- App **Android en Java**: autenticación JWT, modo invitado y multiidioma (ES/EN)
- **Desplegada en dos infraestructuras reales:** **AWS EC2** con nginx como reverse proxy y servicio systemd con reinicio automático, y **Render + Aiven MySQL** con TLS `verify-full` y toda la configuración por variables de entorno
- Tests con JUnit 5, Mockito y Spring Boot Test

🔗 [Ver repositorio](https://github.com/ruubeenn13/TFG-GymProFit)

---

### 🎫 Gestor de Turnos — Enercoop
> Sistema presencial de cola de atención para una cooperativa energética real · En producción

**Stack:** `React 19` `Vite` `Supabase (self-hosted)` `PostgreSQL` `Docker Compose` `Realtime` `Vitest` `nginx` `GitLab CI/CD`

- **Supabase autoalojado** con Docker Compose (13 contenedores): auth, API REST, Edge Functions y lógica de negocio
- PostgreSQL con esquema relacional, **RLS por roles** y RPCs
- Frontend React + Vite con actualizaciones **en tiempo real** vía Supabase Realtime
- **5 perfiles de usuario** (admin, gestor, usuario, kiosko, display), reasignación automática de turnos y módulo de estadísticas
- Multiidioma **ES/VAL/EN** · agente de kiosko independiente · pipeline de CI/CD en GitLab

*Proyecto interno en producción — repositorio privado*

---

### 🧠 iabd-prep — Preparación en IA y Big Data
> Plan de autoformación de 16 semanas antes del curso de especialización

**Stack:** `Python` `MongoDB` `AWS` `Hadoop` `Spark` `Kafka` `Airflow` `Hugging Face`

- Ruta estructurada: Python base → NoSQL → Cloud → Big Data/ETL → Hadoop → Spark → Kafka/NiFi/Airflow → Hugging Face → IoT
- Ejercicios y notebooks propios, con progreso semanal versionado

🔗 [Ver repositorio](https://github.com/ruubeenn13/iabd-prep)

---

<details>
<summary><strong>📁 Otros proyectos</strong></summary>

<br/>

| Proyecto | Descripción | Stack |
|---|---|---|
| **[La Marmita Para Llevar](https://lamarmitaparallevar.com)** | Web corporativa para restaurante de comida para llevar: menú, pedidos, horarios y FAQ. Responsive y desplegada con dominio propio. | `HTML` `CSS` `JavaScript` |
| **[Filmoteca](https://github.com/ruubeenn13/filmoteca-RubenJuan)** | App Android de gestión de colecciones de películas: autenticación, CRUD completo, reproducción multimedia y notificaciones locales. | `Java` `Android` `SQLite` `Material Design` |

</details>

---

## 🛠️ Stack

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

## 🎓 Formación

| | |
|---|---|
| **Especialización en IA y Big Data** · 600 h *(desde oct. 2026)* | IES Severo Ochoa, Elche |
| **CFGS DAM** — Desarrollo de Aplicaciones Multiplataforma | IES Macià Abela, Crevillente · 2024–2026 |
| **CFGM SMR** — Sistemas Microinformáticos y Redes | IES Macià Abela, Crevillente · 2022–2024 |

---

## 📊 Stats

<div align="center">

<img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/0-profile-details.svg" width="90%" alt="Resumen del perfil" />

<img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/3-stats.svg" width="49%" alt="Estadísticas" />
<img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/4-productive-time.svg" width="49%" alt="Horario productivo" />

<img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/1-repos-per-language.svg" width="49%" alt="Repositorios por lenguaje" />
<img src="https://raw.githubusercontent.com/ruubeenn13/ruubeenn13/main/profile-summary-card-output/github_dark/2-most-commit-language.svg" width="49%" alt="Lenguajes más usados" />

</div>

---

## 📫 Contacto

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rubén_Juan_Candela-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/rub%C3%A9n-juan-candela-9743a026a)
[![Email](https://img.shields.io/badge/Email-rubenjuancandela06@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rubenjuancandela06@gmail.com)

</div>
