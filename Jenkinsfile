pipeline {
    agent {
        label 'any'
    }
    stages {
        stage('Validate Release drafter config') {
            steps {
                dir('scripts') {
                    sh 'npm install'
                }
                sh './scripts/validateReleaseDrafterConfiguration.sh'
            }
        }
    }
}
