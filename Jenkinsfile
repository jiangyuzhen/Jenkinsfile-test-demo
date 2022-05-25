pipeline{
    agent any

    tools{
        nodejs 'NodeJS 14.17.0'
    }

    stages {
        stage('Install Packages') {
            steps {
             sh ' node -v & npm version'
             sh 'npm install'
            }
        }

        stage('test and build') {
            steps {
             sh ' npm run test'
             sh 'npm run build'
            }
        }

        stage('deployment') {
            steps {
             echo 'waiting to deployment'
            }
        }
    }
}