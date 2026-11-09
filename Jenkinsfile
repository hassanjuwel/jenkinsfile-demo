pipeline {

    agent any

    stages {

        stage('Credential Test') {

            steps {

                withCredentials([
                    usernamePassword(
                        credentialsId: 'github-token',
                        usernameVariable: 'USERNAME',
                        passwordVariable: 'PASSWORD'
                    )
                ]) {

                    echo 'Credentials Loaded Successfully'

                }

            }

        }

    }

}
