pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
                echo "'${env.BRANCH_NAME}'"
            }
        }
        stage('Example Deploy') {
            when {
                branch 'production'
            }
            steps {
                echo 'Deploying'
            }
        }
    }
}