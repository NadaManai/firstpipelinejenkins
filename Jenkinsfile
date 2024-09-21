pipeline {
    agent any

    triggers {
        pollSCM('H/1 * * * *')
    }

    stages {
        stage('Récupération du code source') {
            steps {
                checkout scm
            }
        }

        stage('Afficher la date système') {
            steps {
                script {
                    echo "Date système : ${new Date()}"
                }
            }
        }

        stage('Exécuter le code') {
            steps {
                // Exécuter le fichier hello.py
                sh 'python3 hello.py'
            }
        }
    }

    post {
        always {
            echo 'Fin du build'
        }
    }
}
