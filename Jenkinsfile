@Library('jenkins-shared-lib') _

pipeline {
    agent any 
    
    stages {
        stage('Git Checkout') {
            steps {
                script {
                    gitCheckout(
                        branch: 'main',
                        url: 'https://github.com/akvd-gitbox/mrdevops_java_app_main.git'
                    )
                }
            }
        }

    stage('Maven Unit test') {
            steps {
                script {
                    mvnTest()
                }
            }
        }
    }
}