  pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project '
            }
        }
        
    stage('Test') {
            steps {
                echo 'Running Tests... '
            }
        }
        
    stage('Deploy') {
            steps {
                echo 'Deploying the application '
            }
        }
    }
    
    post {
        
        success{
            echo 'Pipeline completed successfully'
        }
        failure{
            echo 'Pipeline failed.'
        }
    }
}
