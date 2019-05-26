pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		git branch: 'master', url: 'https://github.com/swagathj/ansibleplaybook-git.git/'
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
		dir('Ansibledemo')
              {
               
               sh 'ansible all -m ping -i inventory'
	     }
            }
        }
    }
}
