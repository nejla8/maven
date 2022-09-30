pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App'
            }
        }
    
    
        stage('Test') {
            steps {
                echo 'Test App'
            }
        }
    
     
        stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
    }
    post{
        failure{
            emailext body: 'summary', subject: 'pipeline status', to: 'snejla@comtrade.com'
        }
    }
}
