pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Récupérer le code source depuis le référentiel Git
                git url: 'https://github.com/NadaManai/firstpipelinejenkins.git'
            }
        }

        stage('Show Date') {
            steps {
                // Afficher la date système
                script {
                    def currentDate = new Date()
                    echo "La date système est : ${currentDate}"
                }
            }
        }
    }

    triggers {
        // Aucune action de déclenchement ici
    }
}
