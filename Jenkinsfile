pipeline {
	agent any

	triggers {
       		pollSCM('*/2 * * * *')
   	}

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

				sh '''sudo cp *.html /var/www/html/ '''
			}

		}

	}
}
