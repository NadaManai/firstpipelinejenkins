pipeline {
    agent any 

    stages {
        stage('Récupération du code source') {
            steps {
                // Récupérer le code depuis le référentiel Git
                git 'https://github.com/NadaManai/firstpipelinejenkins.git'
            }
        }
        stage('Afficher la date système') {
            steps {
                // Afficher la date système
                script {
                    def date = new Date()
                    echo "Date actuelle : ${date.format('yyyy-MM-dd HH:mm:ss')}"
                }
            }
        }
    }
}
