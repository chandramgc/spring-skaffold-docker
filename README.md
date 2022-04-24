# Autodeploy of Spring Boot Application using skaffold into Docker-Desktop

## Prerequisite

For this demo following are required to be installed.

    Installing Dev-Tools (i.e, Java, Gradle, Git, VSCode)
    Installing Skaffold
    Installing Docker Desktop
    Installing kubectl(Optional)
    Minikube(Optional)

## Spring boilerplate

https://start.spring.io/

## Skaffold

### Install Jib plugin

##### build.gradle
```
plugins {
	id 'com.google.cloud.tools.jib' version '3.2.1'
}
```

gradle jibDockerBuild

Add k8s-deploy.yml
Add skaffol.yml

<!-- Build spring boot app -->
skaffold build
<!-- Deploy spring boot app in K8s -->
skaffold run
<!-- Create a live deploy from local to K8s -->
skaffold dev

## Reference Links

https://ashishtechmill.com/cicd-workflow-for-spring-boot-application-on-kubernetes-via-skaffold
