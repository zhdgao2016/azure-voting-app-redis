pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                echo "$GIT_BRANCH"
            }
        }       
        stage('Docker Build') {
            steps {
                sh 'docker images -a'
                sh 'cd azure-vote/'
                sh 'pwd'
                sh 'cd azure-vote/'
                sh 'pwd'
                sh 'docker images -a'
                sh 'docker build -t jenkins-pipeline .'
                sh 'docker images -a'
                sh 'cd ..'                
            }
        }     
    }
}
