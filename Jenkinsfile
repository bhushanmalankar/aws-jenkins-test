pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh 'sudo apt update -y'
                sh 'sudo apt install git -y' 
                sh 'git clone https://github.com/ashishrpandey/maven-project'
                sh 'cd maven-project'
                sh 'mvn compile'
            }
        }
    }
}
