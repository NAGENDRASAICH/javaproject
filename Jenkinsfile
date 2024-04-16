pipeline {
    agent any

    stages {
        stage('Code Checkout') {
            steps {
                git branch: 'master', credentialsId: 'GitHubCreds', url: 'https://github.com/NAGENDRASAICH/myprojectfirst.git'
            }
        }

        stage('Build and Test') {
            steps {
                // Print a success message
                echo 'Build and test succeeded!'

                // Archive the artifact (replace 'target/*.war' with the path to your artifact)
                
            }
        }
    }

    post {
        always {
            // Display a link to download the archived artifact
            archiveArtifacts artifacts: 'target/*.rar', fingerprint: true

            // Cleanup or additional actions that should always run
            echo 'Pipeline execution complete.'
        }
    }
}
