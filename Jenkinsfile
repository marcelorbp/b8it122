#!/usr/bin/env groovy 
pipeline {
    agent any

    tools {
         maven 'maven'
         jdk 'java'
    }

    stages{
        stage('checkout'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'github access', url: 'https://github.com/sreenivas449/java-hello-world-with-maven.git']]])
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
