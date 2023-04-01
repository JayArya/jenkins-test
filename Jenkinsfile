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
                expression {return env.BRANCH_NAME ==~ /(feature\/\w+)/}
            }
            input {
                message "proceed?"
                submitter "ja14871"
                submitterParameter "approver"
            }
            steps {
                echo "'${env.BRANCH_NAME}'"
                echo "'${env.approver}'"
            }
        }
    }
}