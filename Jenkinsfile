pipeline {
    agent any

    stages {
        stage('git') {
            steps {
                git branch: 'main', credentialsId: '145949cf-3ced-4fb1-8af6-2cd8d3f8ffd0', url: 'https://github.com/ugr519/multi.git'
            }
        }
        stage('buld') {
            steps {
               bat "mvn clean package"
            }
        }
        
    }
}
