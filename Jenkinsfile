pipeline {

    agent any

    stages {

        stage('Login') {

            steps {

                withCredentials([
                    usernamePassword(
                        credentialsId: '1b50417c-807f-45dd-b6e9-c3f99c339d2a',
                        usernameVariable: 'USER',
                        passwordVariable: 'PASS'
                    )
                ]) {

                    echo "Username Loaded"

                }

            }

        }

    }

}
