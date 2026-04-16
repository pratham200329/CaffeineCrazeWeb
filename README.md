# Caffeine Craze Web

Caffeine Craze Web is a Jakarta EE web application for a coffee shop workflow with customer ordering, authentication, profile management, and admin dashboards.

## Features

- Customer storefront pages for browsing and ordering
- Shopping cart and order processing flow
- User authentication (login/register)
- User profile view and edit pages
- Admin panel for products, users, orders, analytics, and reports
- MySQL-backed persistence with JDBC
- Password hashing with BCrypt

## Tech Stack

- Java 17
- Jakarta EE (Web Profile APIs via `jakarta.jakartaee-api`)
- JSP + JSTL
- Maven (WAR packaging)
- MySQL 8
- JDBC (MySQL Connector/J)

## Project Structure

- `src/main/java/com/mycompany/caffeinecrazeweb/` : Java source and app configuration
- `src/main/webapp/` : JSP pages, static assets, and SQL seed script
- `src/main/webapp/admin/` : Admin dashboard pages
- `src/main/webapp/auth/` : Authentication pages
- `src/main/webapp/css/` : Stylesheets
- `src/main/webapp/js/` : Frontend scripts
- `src/main/resources/META-INF/persistence.xml` : Persistence configuration
- `pom.xml` : Maven dependencies and build configuration

## Prerequisites

- JDK 17+
- Maven 3.8+
- MySQL Server 8+
- A Jakarta EE compatible application server (for example: GlassFish 7 or Payara 6)

## Database Setup

1. Create a MySQL database named `caffeine_craze`.
2. Import the SQL script from:
   - `src/main/webapp/caffeine_craze.sql`
3. Update database credentials in:
   - `src/main/java/com/mycompany/caffeinecrazeweb/DBConnection.java`

Current defaults in code:

- Host: `localhost`
- Port: `3306`
- Database: `caffeine_craze`
- Username: `root`
- Password: empty

## Build

Run from the project root:

```bash
mvn clean package
```

This generates:

- `target/CaffeineCrazeWeb-1.0-SNAPSHOT.war`

## Run / Deploy

### Option 1: NetBeans

1. Open the project in NetBeans.
2. Configure your Jakarta EE server.
3. Run the project.

### Option 2: Manual deployment

1. Build the WAR with Maven.
2. Deploy `target/CaffeineCrazeWeb-1.0-SNAPSHOT.war` to your server.
3. Open in browser (example):
   - `http://localhost:8080/CaffeineCrazeWeb-1.0-SNAPSHOT/`

## Useful Pages

- Home: `/index.jsp`
- Menu: `/menu.jsp`
- Cart: `/cart.jsp`
- Login: `/auth/login.jsp`
- Register: `/auth/register.jsp`
- Admin: `/admin/index.jsp`

## Notes

- Session timeout is configured in `src/main/webapp/WEB-INF/web.xml`.
- REST base path is configured at `/resources` in `JakartaRestConfiguration`.
- Consider moving DB credentials to environment variables or server configuration for production.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a pull request

## License

Add your preferred license details here (for example MIT, Apache-2.0, or proprietary).
