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
            pwsh(script: 'docker images -a')
            pwsh(script: """
                cd azure-vote/
                docker images -a
                docker build -t jenkins-pipeline .
                docker images-a
                cd ..
            """)
            }
        }
    }
}
