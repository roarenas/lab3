pipeline {
    agent {
        label 'gogo'
    }
    stages{
        stage("Primer paso pipeline") {
            steps{
                sh 'echo "saludos desde el terminal"'
            }
        }
        stage("Segundo paso paso pipeline") {
            agent {
                label 'debian'
            }
            steps{
                sh 'node --version'
            }
        }
        stage("Tercer paso paso pipeline") {
            steps{
                sh 'docker ps'
            }
        }
    }
}