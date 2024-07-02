pipeline {
    agent any
          environment {
                PYTHON_HOME = 'C:/Users/a7200/AppData/Local/Programs/Python/Python312'
                PIP_HOME = 'C:\\Users\\a7200\\AppData\\Local\\Microsoft\\WindowsApps' 
                PATH = "${env.PYTHON_HOME}\\;${env.PIP_HOME};${env.PATH}"
          }
    stages {
        stage('Build') {
            steps {
                script {
                    // Choisissez la commande en fonction de votre script
                    bat 'pip install pandas' // Installer les dépendances
                    bat 'python data_analysis.py' // Exécuter le script Python
                }
            }
        }
    }
}