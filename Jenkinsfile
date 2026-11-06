pipeline {

    agent any

    parameters {

        string(
            name: 'APP_NAME',
            defaultValue: 'MyApp'
        )

        choice(
            name: 'ENV',
            choices: ['DEV','QA','PROD']
        )

    }

    stages {

        stage('Build Information') {

            steps {

                echo "Application: ${params.APP_NAME}"

                echo "Environment: ${params.ENV}"

            }

        }

        stage('System Info') {

            steps {

                bat 'hostname'

                bat 'git --version'

            }

        }

    }

}
