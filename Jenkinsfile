pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting Build'
                sh 'g++ -o pes2ug20cs043.exe hello.cpp'
                echo 'Build Completed'
            }
        }
        stage('Test') {
            steps {
                eco 'Starting Testing'
                sh './pes2ug20cs043.exe'
                echo 'Test Completed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Starting Deploy'
                echo 'Deploy Completed'
            }
        }
    }
  post {
    failure {
      echo 'Pipeline Failed'
    }
  }
}
