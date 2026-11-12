pipeline {                                    // Déclare un pipeline déclaratif
    agent any                                 // Exécute sur n'importe quel agent disponible

    stages {                                  // Liste des étapes, exécutées dans l'ordre
        stage('Git clone') {                  // Étape 1 : récupération du code
            steps {
                git branch: 'main',           // Branche à récupérer
                    credentialsId: 'GIT_HUB_CREDENTIALS',   // Identifiant GitHub stocké dans Jenkins
                    url: 'https://github.com/hero25-h/DevOps-AppGestionDesProjetsHM.git'
            }
        }

        stage('Build') {                      // Étape 2 : construction du projet
            steps {
                sh 'echo "Build du projet"'   // À remplacer par les vraies commandes de build
            }
        }
    }
}
