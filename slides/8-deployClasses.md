### Deploying Files.

`build.gradle`:

    plugins {
        id "org.hidetake.ssh" version "2.9.0"
    }
    
    ...
    
    task deployClasses(dependsOn: ...){
        ssh.run {
            session(remotes.oracleEBS){
                put from: javaClasses, into: java_top
            }
        }
    }    
    
    ...