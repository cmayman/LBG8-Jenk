pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''chmod +x helloworld.sh
                ./helloworld.sh'''
            }
        }
        stage('Archive Files') {
            steps {
                sh '''/usr/games/cowsay "moo" > ourcowsays.txt
                '''
            }
        }
    }
}