#!/usr/bin/env groovy 
pipeline {
    agent any

    tools {
         maven 'MAVEN'
    }

    stages{
        stage('Checkout'){
            steps{
                 git changelog: false, poll: false, url: 'https://github.com/marcelorbp/b8it122.git'
            }
        }
        stage('Build') { 
            steps {
                // 
               echo 'Build...'
               bat 'mvn package'
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
