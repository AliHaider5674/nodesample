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
                sh 'npm install'
            }
        }
    }
    stage("Build Docker") {
        steps {
            catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
                script {
                    // here want to call function from another file
                   load("commonFunctions.groovy").buildDocker(par1, par2)
                }
            }
        }
    }
}
