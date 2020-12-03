pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                //snDevOpsStep()
                echo 'Hello, Build'
            }
        }
        stage('UAT deploy') {
            steps {
                //snDevOpsStep()
                echo 'Hello, UAT deploy'
                }
        }
        if (true) {
            stage('UAT test') {
                steps {
                    //snDevOpsStep()
                    echo 'Hello, UAT test'
                }
            }
        }
        stage('Prod Deploy') {
            steps {
                //snDevOpsStep()
                snDevOpsChange()
                echo 'Hello, Prod Deploy'
            }
        }
    }
}
