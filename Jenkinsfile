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
            xunit (
                thresholds: [ skipped(failureThreshold: '0'), failed(failureThreshold: '0') ],
                tools: [ GoogleTest(pattern: '**/*.xml') ])
        }
    }
 }
