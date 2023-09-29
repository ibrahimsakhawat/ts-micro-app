pipeline {
    agent any 
    stages {
        stage('Checkout') {
            steps {
                
                checkout scm
            }
        }
        
        stage('Yarn Install') {
            steps {
                
                bat 'yarn install'
            }
        }
    }

    post {
        success {
            
            echo 'Yarn install succeeded'
        }

        failure {
          
            echo 'Yarn install failed'
        }
    }
}