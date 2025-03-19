pipeline {
    agent any

    stages {
        stage('Setup Flutter') {
            agent {
                docker {
                    image 'cirrusci/flutter:stable'  
                   
                }
            }
            steps {
                sh '''
                flutter --version
                flutter doctor
                '''
            }
        }
    }
}