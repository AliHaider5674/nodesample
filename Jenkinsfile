#!/usr/bin/env groovy

pipeline {

    agent {
        docker {
            image 'node'
            args '-u root'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                pipeline = load 'commonFunctions.groovy'
                pipeline.buildDocker(par1, par2)
            }
        }
    }
}
