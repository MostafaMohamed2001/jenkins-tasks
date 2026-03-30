pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git credentialsId: 'github-creds',
                    url: 'https://github.com/MostafaMohamed2001/jenkins-tasks'
            }
        }

        stage('Run Script') {
            steps {
                sh 'chmod +x scripts.sh'
                sh './scripts.sh'
            }
        }
    }
}