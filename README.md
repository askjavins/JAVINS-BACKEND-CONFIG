# JAVINS Backend configuration

Environment-specific Spring Boot configuration for `askjavins/JAVINS-BACKEND`.

These files intentionally contain no secrets. Database, SMTP, JWT, WhatsApp,
and encryption values are supplied to the deployed container as environment
variables. The backend deployment workflows fetch the matching file and copy
it to `src/main/resources/application.yml` immediately before the Docker build.
