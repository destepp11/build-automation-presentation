### Flyway Properties 

`build.gradle`:

    flyway {
        url = props.getProperty("flyway.url")
        driver = props.getProperty("flyway.driver")
        user = props.getProperty("flyway.user")
        password = props.getProperty("flyway.password")
        table = props.getProperty("flyway.table")
        baselineOnMigrate = props.getProperty("flyway.baselineOnMigrate")
    }