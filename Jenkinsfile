pipeline {
    agent any
          environment {
                PYTHON_HOME = 'C:/Users/a7200/AppData/Local/Programs/Python/Python312'
                PATH = "${env.PYTHON_HOME}\\;${env.PATH}"
          }
    stages {
        stage('Build') {
            steps {
                script {
                    // Choisissez la commande en fonction de votre script
                    bat 'python -m pip install pandas' // Installer les dépendances
                    bat 'python data_analysis.py' // Exécuter le script Python
                }
            }
        }
    }
}