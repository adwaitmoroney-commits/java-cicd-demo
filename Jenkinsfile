pipeline {

    agent any


    stages {


        stage('Build Application') {

            steps {

                sh 'mvn clean package'

            }

        }


        stage('SonarQube Analysis') {

            steps {

                echo 'Running SonarQube Analysis'

            }

        }

    }


    post {

        success {

            echo 'Build Completed Successfully'

        }

        failure {

            echo 'Build Failed'

        }

    }

}
 
