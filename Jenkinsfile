pipeline {

  agent any

 

  stages {

    stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/abhaypawa/jenkins_project.git'
            }
        }

    stage('Install Dependencies') {

      steps {

        bat 'npm install'

      }

    }

    stage('Run Tests') {

      steps {

        bat 'npm test'

      }

    }

  }

}