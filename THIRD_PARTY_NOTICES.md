# Third-party notices

IKM is proprietary software (see [LICENSE](LICENSE)). It includes the open-source components below, each under its own license. Nothing in the IKM license limits your rights under these licenses.

The license and NOTICE files that come with each Java library stay inside the library's own jar, unchanged, in `app.jar` (`BOOT-INF/lib/`).

## Backend (`app.jar` in the `ikm-app` image)

| Component | License |
|---|---|
| Spring Framework, Spring Boot, Spring Data, Spring Security | Apache-2.0 |
| Hibernate ORM, Hibernate Models, Hibernate Validator, JBoss Logging, Classmate | Apache-2.0 |
| Apache Tomcat (embedded), Apache Commons Lang, Apache Commons Logging, Apache Log4j API and to-SLF4J bridge | Apache-2.0 |
| Jackson (2 and 3), SnakeYAML, Byte Buddy, HikariCP, Micrometer, JSpecify, Jakarta Inject API, Jakarta Validation API | Apache-2.0 |
| Flyway (community edition, PostgreSQL support) | Apache-2.0 |
| springdoc-openapi, Swagger Core, Swagger UI | Apache-2.0 |
| PostgreSQL JDBC driver | BSD-2-Clause |
| HdrHistogram | BSD-2-Clause (or CC0-1.0) |
| ANTLR 4 runtime | BSD-3-Clause |
| SLF4J, jul-to-slf4j, Checker Framework qualifiers, webjars-locator-lite | MIT |
| Logback | EPL-1.0 / LGPL-2.1 (dual; used under EPL) |
| AspectJ weaver | EPL-2.0 (with BSD-3-Clause and Apache-1.1 parts) |
| Jakarta Annotation API, Jakarta Transaction API | EPL-2.0 or GPL-2.0 with Classpath Exception |
| Jakarta Persistence API | EPL-2.0 / EDL-1.0 |
| Jakarta Activation, Jakarta XML Binding (API and runtime), Angus Activation, istack, TXW2 | EDL-1.0 (BSD-3-Clause) |

## Tablet app and admin page (served by the `ikm-app` image)

Bundled, minified, into the app's JavaScript file:

| Component | License |
|---|---|
| React, React DOM, scheduler | MIT |

Fonts:

| Font | License |
|---|---|
| Plus Jakarta Sans, Copyright 2020 The Plus Jakarta Sans Project Authors | SIL Open Font License 1.1 |

The full font license is in `web/src/assets/fonts/OFL-PlusJakartaSans.txt`, in the repository and in the release zip.

## Docker images

The release zip's `ikm-images.tar.gz` holds one image built on an open-source base:

| Image | Built on | Includes |
|---|---|---|
| `ikm-app` | `eclipse-temurin:25-jre-alpine` | Eclipse Temurin Java runtime (OpenJDK, GPL-2.0 with Classpath Exception) and Alpine Linux packages (among others BusyBox, GPL-2.0; musl libc, MIT) |

The database is not in the zip. The installer downloads the official `postgres:15` image (PostgreSQL License) from Docker Hub; the backup service uses the same image.

### Source code of GPL and LGPL components

The source code of the GPL- and LGPL-licensed components above is published by their projects:
- Eclipse Temurin: https://github.com/adoptium
- Alpine Linux packages: https://gitlab.alpinelinux.org/alpine/aports

For three years from the date you received IKM, the Licensor will also provide, on request, a copy of the corresponding source code of those components, for no more than the cost of making and sending it. Ask your IKM supplier, who passes the request to the Licensor.
