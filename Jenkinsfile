pipeline {
        agent none
        stages {
         
          stage("build & SonarQube Scanner") {
            agent any
            steps {
              withSonarQubeEnv('Sonar_token') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
