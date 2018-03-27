### Load Properties

`build.gradle`:

    loadConfiguration()
    
    def loadConfiguration() {
        def environment = project.hasProperty('env') ? project.env : 'dev'
        project.ext.set 'environment', environment
        println "Environment is set to $environment"
    
        def configFile = file('config.groovy')
        def config = new ConfigSlurper(environment).parse(configFile.toURI().toURL())
        project.ext.set 'config', config
    }
    
    def props = new Properties()
    file("$config.instanceProperties").withInputStream { props.load(it) }