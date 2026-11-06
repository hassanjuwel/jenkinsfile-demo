pipeline {

    agent any

    parameters {

        string(
            name: 'USERNAME',
            defaultValue: 'Admin'
        )

    }

    stages {

        stage('Welcome') {

            steps {

                bat "echo Welcome ${params.USERNAME}"

            }

        }

    }

}
