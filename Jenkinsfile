pipeline {
    agent any

    stages {
        stage('Verify branch') {
            steps {
                echo "$GIT_BRANCH" 
            }
        }
        stage('docker build') {
            steps{
            sh(script: 'docker images -a')
            sh(script: """
                cd azure-vote/
                docker images -a
                cd ..
            """)
            }
        }
    }
}
