#!/usr/bin/env groovy
pipeline {
    agent any

    stages {
        stage("Run tests") {
            steps {
                echo "*******testing************"
                sh 'pytest'
            }
        }
    }
}
