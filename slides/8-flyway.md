### Flyway Properties 

`local.properties`:

    flyway.url = jdbc:oracle:thin:@//localhost/local
    flyway.driver = oracle.jdbc.driver.OracleDriver
    flyway.user = apps
    flyway.password = apps
    flyway.table = schema_version
    flyway.baselineOnMigrate = true