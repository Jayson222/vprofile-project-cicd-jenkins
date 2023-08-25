pipeline {
        agent any                                                                                                             tools {                                                                                                                       maven "maven3"
                jdk "openjdk8"
        }

        environment {
                SNAP_REPO = 'vprofile-snapshot'
                NEXUS_USER = 'admin'
                NEXUS_PASS = 'admin'
                RELEASE-REPO = 'vprofile-release'
                CENTRAL_REPO = 'vpro-maven-central'
                NEXUSIP = '13.54.47.86'
                NEXUSPORT = '8081'
                NEXUS_GRP_REPO = 'vprofile-group'
                NEXUS_LOGIN = 'nexuslogin'
        }

        stages {
              stage(build){
                step{
                  sh 'mvn -s settings.xml -DskipTests install'
                }
        }
}
