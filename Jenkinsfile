#!/usr/bin/env groovy

#Jenkinsfile
pipeline{
	
	agent{
		docker {
			image 'maven'
			label 'my-pipeline-test'
			args '-u vagrant'
			}
	}

	stages{
		stage('Build'){
			steps{
				echo "Building..."
				sh 'mvn package'
			}
		}
	}
}