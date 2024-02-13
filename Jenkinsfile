node {
   stage('clone') {
    git 'https://github.com/bmimen/Jenkins.git'
     }
     stage('build') {
	   sh lable:'', script:'javac Main.java'
     }
    stage('run') {
    sh lable:'', script:'java Main'
}
}
