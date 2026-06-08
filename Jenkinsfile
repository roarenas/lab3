pipeline {
    agent {
        label 'debian'
    }
    stages{
        stage("Primer paso pipeline") {
            steps{
                sh 'echo "saludos desde el terminal"'
            }
        }
        stage("Segundo paso paso pipeline") {
            steps{
                sh 'pwd'
                sh 'export'
                sh 'node --version'
            }
        }
        stage("Tercer paso paso pipeline") {
            agent {
                label 'Gogo'
            }
            steps{
                sh 'docker ps'
            }
        }
    }
}