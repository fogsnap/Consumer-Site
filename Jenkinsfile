pipeline {
    agent any
    
    parameters {
        booleanParam(name: "DEPLOY", defaultValue: true)
    }

    stages {
        stage('Build') {
            steps {
                //snDevOpsStep()
                echo 'Hello, Build'
            }
        }
        stage('UAT deploy') {
            when { expression { params.DEPLOY} }
            steps {
                //snDevOpsStep()
                echo 'Hello, UAT deploy'
                }
        }
        stage('UAT test') {
            steps {
                //snDevOpsStep()
                echo 'Hello, UAT test'
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
