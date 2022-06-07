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
                load("commonFunctions.groovy").buildDocker(par1, par2)
            }
        }
    }
}
