/*@Library('my-shared-library2@main') _

jenkinsfile{
message = "hello world it is my jenkins call from another repo"
}
*/
pipeline {
    agent { label 'agent' }

    stages {
        stage('Build') {
            steps {
                script {
                    echo "agent is working"
                }
            }
        }
    }
}
