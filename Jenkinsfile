pipeline {

    agent any

    

    stages {

        stage('SCM code') {

            steps {

                git 'https://github.com/amitvermaa93/jenkins-git-integration.git'

            }

        }

        

        stage('Build') {

            steps {

                sh 'mvn clean package'

            }

        }

        stage('Publish') {

            steps {

                // Add steps to publish artifacts or deploy the application

                // For example, you can use the 'archiveArtifacts' step to archive built artifacts

                archiveArtifacts 'target/*.war'

            }

        }

    }

}
