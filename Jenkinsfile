pipeline {
 agent any
  stages {
      stage('Checkout') {
         steps {
            git 'https://github.com/Devops-trainer1987/ctsjune22021.git'
         }
      }
       stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "C:/Windows/System32/config/systemprofile/AppData/Local/Jenkins/.jenkins/workspace/cts_pipeline/target/cts-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
