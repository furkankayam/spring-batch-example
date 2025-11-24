# ⚙️ Spring Batch Example

<div>
<div align="center">
<h3> Project Architecture </h3>
<img src="./images/project-architecture.png" alt="Project Architecture">
</div>

### Project Summary:

- Triggered within the campaign management processes, this module executes bulk email notifications to the target audience using the Spring Batch architecture. The system relies on the Chunk-Oriented Processing model to ensure resource optimization and transactional integrity. Each cycle processes data in blocks of 100 records , enabling high-volume email delivery in a performant and controlled manner while minimizing database load.

<br>

---

### Tech Stack:

[![Java](https://img.shields.io/badge/java-17.0-000?style=for-the-badge&logo=openjdk&logoColor=white&color=FF9A00)](https://www.java.com/en/)
[![JavaScript](https://img.shields.io/badge/javascript-000?style=for-the-badge&logo=javascript&logoColor=black&color=F7DF1E)](https://ecma-international.org/)
[![Spring Boot](https://img.shields.io/badge/spring%20boot-3.5.7-000?style=for-the-badge&logo=springboot&logoColor=white&color=6DB33F)](https://spring.io/)
[![Spring Batch](https://img.shields.io/badge/spring%20batch-3.5.7-000?style=for-the-badge&logo=spring&logoColor=white&color=6DB33F)](https://spring.io/projects/spring-batch)
[![Apache FreeMarker](https://img.shields.io/badge/apache%20freemarker-3.5.7-000?style=for-the-badge&logo=apachefreemarker&logoColor=white&color=326CAC)](https://freemarker.apache.org/)
[![NextJS](https://img.shields.io/badge/nextjs-3.5.7-000?style=for-the-badge&logo=next.js&logoColor=white&color=000000)](https://nextjs.org/)
[![TailwindCSS](https://img.shields.io/badge/tailwindcss-4.0-000?style=for-the-badge&logo=tailwindcss&logoColor=white&color=06B6D4)](https://tailwindcss.com/)
[![Mapstruct](https://img.shields.io/badge/Mapstruct-1.6.3-000?style=for-the-badge&logo=mapstruct&logoColor=white&color=FABF15)](https://mapstruct.org/)
[![Gradle](https://img.shields.io/badge/Gradle-9.2-000?style=for-the-badge&logo=gradle&logoColor=white&color=02303A)](https://gradle.org/)
[![Flyway](https://img.shields.io/badge/Flyway-11.17-000?style=for-the-badge&logo=flyway&logoColor=white&color=CC0200)](https://www.red-gate.com/products/flyway/community/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15.2-000?style=for-the-badge&logo=postgresql&logoColor=white&color=4479A1)](https://www.postgresql.org/)
[![Open API](https://img.shields.io/badge/Open%20API-2.8-000?style=for-the-badge&logo=openapiinitiative&logoColor=white&color=6BA539)](https://springdoc.org/)
[![Docker](https://img.shields.io/badge/Docker-28.3-000?style=for-the-badge&logo=Docker&logoColor=white&color=2496ED)](https://docs.docker.com/)
[![Docker Compsose](https://img.shields.io/badge/Docker%20Compose-3.7-000?style=for-the-badge&logo=Docker&logoColor=white&color=2496ED)](https://docs.docker.com/compose/)

<br>

---

### 🚀 Setup

#### Database Configuration

- **PostgreSQL**
  - **URL:** `http://localhost:5432`
  - **Database:** `batch_db`
  - **Username:** `postgres`
  - **Password:** `postgres`

<br>

#### Mail Configuration

```yaml
# Mail Config
spring:
  mail:
    host: smtp.gmail.com
    port: 587
    username: <email>
    password: <password>
    properties:
      mail:
        smtp:
          auth: true
          starttls:
            enable: true
```

<br>

#### Start Services with Docker Compose

```bash
docker-compose up -d
```

<br>

---

### 📚 API Documentation

#### 👥 User Management

<details>
<summary>➕ Create User </summary>

![Create User](./images/create-user.png)

</details>

<details>
<summary>📋 Get Users </summary>

![Get Users](./images/main.png)

</details>

<br>

#### 📢 Campaign Management

<details>
<summary>➕ Create Campaign </summary>

![Create Campaign](./images/create-campaign.png)

</details>

<details>
<summary>📤 Campaign Request </summary>

![Campaign Request](./images/campaign-request.png)

</details>

<br>

#### 📧 Email Operations

<details>
<summary>✉️ Email Preview </summary>

![Email Preview](./images/mail.png)

</details>

<br>

#### 📖 OpenAPI Documentation

<details>
<summary>📄 OpenAPI Specification </summary>

![OpenAPI](./images/openapi.png)

</details>

<br>

### 🐳 Docker Interface

<details>
<summary>🐋 Container Management </summary>

![LazyDocker](./images/docker.png)

</details>

<br>

---

### 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details

**Created by** [Mehmet Furkan KAYA](https://www.linkedin.com/in/mehmet-furkan-kaya/)
