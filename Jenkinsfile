pipeline {
    agent any
	 stages {
   stage('clone') {
       git credentialsId: '81ef6d50-6daf-4ab2-9c92-11190ca08b7f', 
       branch: 'main', url: 'https://github.com/bmimen/Jenkins.git'
     }
     stage('build') {
	  bat '''javac Main.java
    
'''
     }
  stage('run') {
  bat '''java Main
    
'''
}
}
 post {
        failure {
            // Actions en cas d'échec des tests unitaires
            echo "Les tests unitaires ont échoué sur le serveur A. Veuillez vérifier les rapports de test."

            // Ajoutez des actions supplémentaires si nécessaire, par exemple, notifier une équipe spécifique.
        }
        success {
            // Actions en cas de succès des tests unitaires
            echo "Les tests unitaires ont réussi sur le serveur A. La construction est prête pour la validation manuelle."
        }
    }
	
 }
	
