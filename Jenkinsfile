pipeline{
	agent any
	tools {nodejs "node"}
	stages{
		stage('Install Dependencies'){
			steps{
				sh 'npm install'
			}
		}
		
		stage('Fix'){
			steps{
				sh 'npm audit fix'
			}
		}

		stage('Start'){
			steps{
				sh 'npm start'
			}
		}
	}
}
