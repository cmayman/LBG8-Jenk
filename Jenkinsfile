pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''chmod +x helloworld.sh
                ./helloworld.sh'''
            }
        }
                stage('Make Directoy') {
            steps {
                sh ''' if [[ -d ~/jenkins-tutorial-test ]]
                then echo "directory exists"
                else mkdir ~/jenkins-tutorial-test
                fi
                '''
            }
        }
                stage('Create Files') {
            steps {
                sh '''touch ~/jenkins-tutorial-test/file1 ~/jenkins-tutorial-test/file2
                '''
            }
        }
        stage('Archive Files') {
            steps {
                sh '''/usr/games/cowsay "moo" > /tmp/ourcowsays.txt
                '''
            }
        }
    }
}