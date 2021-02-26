properties([pipelineTriggers([githubPush()])])

pipeline {
    agent {
        label 'github-ci'
    }
    stages {
        stage('Checkout SCM') {
            steps {
               git branch: 'uat', credentialsId: '375811b9-fcb2-48df-b525-2219316ec8d3', url: 'https://github.com/ishitadevops/java.git'
            }
        }
        
        stage('compile code') {
            steps {
                echo 'compile code'   
            }
        }
        
        stage('deploy code'){
            steps {
                echo 'deploy the code on uat'
            }
        }
    }
}
