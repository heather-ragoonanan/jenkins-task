pipeline {
    agent any

    stages {
        stage('Prep') {
            steps {
                echo 'Preparing the workspace...'
                sh 'ls -la'
                sh 'pwd'
            }
        }

        stage('Build Images') {
            steps {
                echo 'Building images...'
                sh 'touch image1.img image2.img'
                sh 'ls -la'
            }
        }

        stage('Run') {
            steps {
                echo 'Running the application...'
                sh 'mv image1.img deployed_image1.img'
                sh 'ls -la'
            }
        }
    }
}
