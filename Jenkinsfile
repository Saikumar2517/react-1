pipeline {
    agent any

    tools {
        // Define Node.js and npm installations
        nodejs 'node' // Name of the Node.js tool in Jenkins configuration
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout your Git repository
                git credentialsId: 'b2f40516-fe7e-4d00-b5c7-a40cf058cc2c', url: 'https://github.com/Saikumar2517/react-1.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install project dependencies
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                // Build the React application
                sh 'npm run build'
            }
        }
    }

}
