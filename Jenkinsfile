pipeline {

    agent any

    stages {

        stage('Credential Test') {

            steps {

                withCredentials([
                    string(
                        credentialsId: '1b50417c-807f-45dd-b6e9-c3f99c339d2a',
                        variable: 'TOKEN'
                    )
                ]) {

                    bat 'echo Credential Loaded'

                }

            }

        }

    }

}
