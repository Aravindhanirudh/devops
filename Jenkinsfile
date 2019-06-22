pipeline {
	agent any
	environment {
		myName="aravindh"
}

	stages{
		stage (checkout) {
			steps {

				git credentialsId: 'github', url: 'https://github.com/Aravindhanirudh/devops.git'
			}

		}
		stage (deployment) {
			steps {

				sh '''cp *.html /var/www/html/ '''
			}

		}

	}
}
