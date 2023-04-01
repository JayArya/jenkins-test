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
                expression {return env.BRANCH_NAME ==~ 'feature/*'}
            }
            steps {
                echo "'${env.BRANCH_NAME}'"
            }
        }
    }
}