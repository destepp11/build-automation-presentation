### Compile Java

`build.gradle`:

    plugins {
        id "java"
    }
    
    group 'rsccorp.radiosys.com'
    version '1.0-SNAPSHOT'
    sourceCompatibility = 1.9
    
    repositories {
        mavenCentral()
    }
    
    dependencies {
        testCompile group: 'junit', name: 'junit', version: '4.12'
    }