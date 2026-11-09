pipeline {

    agent any

    stages {

        stage('Credential Test') {

            steps {

                withCredentials([
                    string(
                        credentialsId: 'juwel',
                        variable: 'TOKEN'
                    )
                ]) {

                    bat 'echo Credential Loaded'

                }

            }

        }

    }

}
