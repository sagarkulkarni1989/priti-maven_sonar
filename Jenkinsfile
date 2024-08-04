pipeline {
        agent any
        stages {
         
          stage("build & SonarQube Scanner") {
            steps {
              withSonarQubeEnv('Sonar_token') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
