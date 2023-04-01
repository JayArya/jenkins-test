pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
                echo '${BRANCH_NAME}'
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