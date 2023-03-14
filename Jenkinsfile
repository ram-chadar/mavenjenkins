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
                ech 'Test App'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
    }
    
    post { 
        always { 
            emailext attachLog: true, body: 'testing...', subject: 'Pipeline Post Mail', to: 'salikramchadar@gmail.com'
        }
    }
}
