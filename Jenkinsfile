pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/bkrraj/game-of-life.git'
            }
        }
    stage('Build') {
      steps {
        echo '<--------------- Building --------------->'
        sh 'printenv'
        sh '/opt/apache-maven-3.9.0/bin/mvn clean install'
        echo '<------------- Build completed --------------->'
      }
    }
    }
}