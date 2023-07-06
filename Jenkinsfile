pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                echo $GIT_BRANCH 
            }
        }
        stage('tchao') {
            steps {
                echo 'Tchao'
            }
        }
        
        stage('ola file helo') {
            steps {
               fileExists 'hello.c'
            }
        }
        
        
        
        
    }
}
