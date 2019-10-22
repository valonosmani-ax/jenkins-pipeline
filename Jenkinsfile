pipeline {
    agent any
    stages {
        stage('Checout'){
            steps {
                echo 'Checking out source code'
				git url: 'https://github.com/predic8/simple-jenkins2'
            }
        }
    }
    post {
        always{
            
        }
    }
 }
