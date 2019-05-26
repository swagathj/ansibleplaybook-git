#!groovy
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
		
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
#		sh 'ansible all -m ping -i /var/lib/jenkins/workspace/Ansibledemo/inventory'
            }
        }
    }
}
