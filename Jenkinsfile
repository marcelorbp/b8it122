#!/usr/bin/env groovy 
pipeline {
    agent any

    tools {
         maven 'MAVEN'
    }

    stages{
        stage('Checkout'){
            steps{
                 checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [url: 'https://github.com/marcelorbp/b8it122.git']])
            }
        }
        stage('Build') { 
            steps {
                // 
               echo 'Build...'
            }
        }
        stage('Test') { 
            steps {
                //
               echo 'Test...'
            }
        }
        stage('Deploy') { 
            steps {
                // 
               echo 'Deploy...'
            }
        }
        stage('Monitor') { 
            steps {
                // 
               echo 'Monitor...'
            }
        }
    }
}
