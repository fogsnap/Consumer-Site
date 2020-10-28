pipeline {
    agent any
    tools { 
        maven 'Jenkins Maven' 
    }
    stages {
        stage('Build') {
            steps {
                snDevOpsStep()
                echo 'Hello, Build'
            }
        }
        stage('UAT deploy') {
            steps {
                snDevOpsStep()
                echo 'Hello, UAT deploy'
                }
        }
        stage('UAT test') {
            steps {
                snDevOpsStep()
                echo 'Hello, UAT test'
            }
        }
        stage('Prod Deploy') {
            steps {
                snDevOpsStep()
                snDevOpsChange()
                echo 'Hello, Prod Deploy'
            }
        }
    }
}
