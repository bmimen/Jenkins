node {
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
