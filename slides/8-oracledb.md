### Creating the Build Script

`build.gradle`:

    repositories {
        mavenCentral()
        mavenLocal()
    }
    
    dependencies {
        compile("com.oracle:ojdbc6:11.2.0.4")
        testCompile group: 'junit', name: 'junit', version: '4.12'
    }
    