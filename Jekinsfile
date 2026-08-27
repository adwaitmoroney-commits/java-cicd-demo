pipeline {

    agent any


    stages {


        stage('Checkout Code') {

            steps {

                git 'https://github.com/adwaitmoroney-commits/java-cicd-demo.git'

            }

        }


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
 
