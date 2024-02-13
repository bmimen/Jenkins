node {
   stage('clone') {
       git credentialsId: '81ef6d50-6daf-4ab2-9c92-11190ca08b7f', url: 'https://github.com/bmimen/Jenkins.git'
     }
     stage('build') {
	   sh lable:'', script:'javac Main.java'
     }
    stage('run') {
    sh lable:'', script:'java Main'
}
}
