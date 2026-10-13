pipeline {
    agent any

    triggers {
        pollSCM('* * * * *')       // vérifie GitHub chaque minute → build seulement s'il y a un nouveau commit
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm       // récupère le code du dépôt configuré dans le job
            }
        }
        stage('Date') {
            steps {
                sh 'date'          // affiche la date système
            }
        }
    }
}
