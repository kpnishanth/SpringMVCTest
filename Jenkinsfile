pipeline {
    agent any

    stages {
        stage("Clean Up"){
            steps{
                deleteDir()
            }
        }

        stage("Build"){
            steps{
                dir("SpringMVCTest"){
                    sh "mvn clean install"
                }
            }
        }
        stage("Test"){
            steps{
                dir("SpringMVCTest"){
                    sh "mvn test"
                }
        }        
    }
}}
