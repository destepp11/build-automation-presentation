### VCS Triggers To Begin Builds

![Build Trigger](images/slides/ciserver/vcsTrigger.PNG)

When the `develop` branch is updated the build step executed is
 
    build -Penv=dev flywayMigrate