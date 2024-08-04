pipeline {
        agent any
        stages {
         
          stage("build & SonarQube Scanner") {
            steps {
              withSonarQubeEnv('SonarQube_Scanner') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
