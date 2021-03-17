#!/usr/bin/env groovy
pipeline {
    agent any

    stages {
        stage("checkout") {
            steps {
                echo "*************checkout************"
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/dkoren-amat/test.git']]])
            }
        }
        stage("Run tests") {
            steps {
                echo "*******testing************"
                sh 'test_add'
            }
        }
    }
}
