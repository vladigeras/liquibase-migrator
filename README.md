# Description
This project is a sample of using database migrator such as a [Liquibase](https://www.liquibase.org) 
for creating standalone application-migrator for you system.

DataSource connection settings are in **resources/application.yml**. There are a simple Spring DataSource
configuration. Now migrator is used for perform migrations to a [PostgreSQL](https://www.postgresql.org) database, but
you can simple change it by adding some jdbc driver to **pom.xml** and change DataSource configuration.

Then application start, Spring create a Liquibase bean, which perform a migrations from **resources/db**.

**changelog-master.xml** is a main migration descriptor.
