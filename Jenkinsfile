/*@Library('my-shared-library2@main') _

jenkinsfile{
message = "hello world it is my jenkins call from another repo"
}
*/
pipeline {
    agent { label 'Built-in Node' }

    stages {
        stage('Build') {
            steps {
                script {
                    echo "agent is working fine"
                }
            }
        }
    }
}
