pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Deploy') {
            when {
                branch 'feature/*'
            }
            steps {
                echo 'Deploying'
            }
        }
    }
}