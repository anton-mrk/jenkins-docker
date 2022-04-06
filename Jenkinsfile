pipeline {
	agent any

	stages {
		stage('Build docker'){
			steps {
				echo "Build docker image"
				sh "docker build -t antonmrk/hm7 ."
			}
		}
		stage('Push image to dockerhub'){
			steps {
				echo "Push docker image to dockerhub"
				sh "docker push antonmrk/hm7"
			}
		}
	}
}
