pipeline {
	agent any
	stages {
		stage('Upload to AWS') {
			steps {
				withAWS(region:'ap-southeast-2', credentials: 'aws-static'){
					s3Upload(bucket:"jenkins-vikram-rajan", , includePattern:'*.html')
				}
			}
		}
	}
}
