pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('fork') {
        	steps {
			sh 'echo "this is from the jenkinsfile"'
			sh 'bash buildbash.sh'
            	}
        }
	stage('test') {
		steps{
			sh 'bash testbash.sh'		
		}
	}
    }
}
