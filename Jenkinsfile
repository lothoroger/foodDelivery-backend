pipeline {

	agent any
	
	stages {
		stage('Build') {
			steps {
			//Get code from GitHub repository
			git (branch: 'main', url: 'https://github.com/lothoroger/capstone2023fdsfood.git')
			
			//Run maven wrapper - 2/20
			//bat  "mvn compile"
			sh "mvn compile"
			echo 'Building the Food Delivery Project with Maven compiler'			
			       }
		               }
		
		stage('Test') {
			steps {
			//bat 'mvn test'
			sh "mvn test"
			echo 'Testing the Food Delivery project with Maven test'
			  }
			       }
		
		stage('Deploy') {
			steps {
			//bat 'mvn package'
			sh "mvn package"
			echo 'Deploy the Food Delivery project with Maven package'
				  }			
						}

	}
}
