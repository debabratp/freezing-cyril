#!/usr/bin/env groovy

pipeline{
	
	agent{
		docker {
			image 'maven'
			//label 'my-pipeline-test'
			args '-u root'
			alwaysPull true
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