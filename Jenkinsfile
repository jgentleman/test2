pipeline {
    agent any {
    stages {
        stage("Compile Stage"){
          steps {
            withMaven(maven : 'maven3') {
            sh 'mvn clean compile'
            }
          }
        }
        stage("Test Stage"){
        steps {
            withMaven(maven : 'maven3') {
            sh 'mvn test'
            }
           }
        }
        stage("Deploy Stage"){
        steps {
            withMaven(maven : 'maven3') {
            sh 'mvn deploy'
            }
           }
        }

        }
    }
}
