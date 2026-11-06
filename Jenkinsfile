pipeline {

    agent any

    environment {

        APP_NAME = 'JenkinsTraining'

    }

    stages {

        stage('Build Info') {

            steps {

                echo "Build Number: ${env.BUILD_NUMBER}"

                echo "Application: ${env.APP_NAME}"

            }

        }

        stage('Workspace') {

            steps {

                bat 'dir'

            }

        }

    }

}
