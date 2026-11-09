pipeline {

    agent any

    parameters {

        choice(
            name: 'ENVIRONMENT',
            choices: ['DEV','QA','PROD'],
            description: 'Select Environment'
        )

    }

    environment {

        APP_NAME = 'JenkinsTraining'

        VERSION = '1.0.0'

    }

    stages {

        stage('Build Information') {

            steps {

                echo "Application: ${env.APP_NAME}"

                echo "Version: ${env.VERSION}"

                echo "Environment: ${params.ENVIRONMENT}"

            }

        }

        stage('System Information') {

            steps {

                bat 'hostname'

                bat 'git --version'

            }

        }

        stage('Credential Test') {

            steps {

                withCredentials([
                    string(
                        credentialsId: 'github-token',
                        variable: 'TOKEN'
                    )
                ]) {

                    echo 'Credential Loaded Successfully'

                }

            }

        }

    }

}
