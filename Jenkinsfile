    node('JDK8') {
        stage('SourceCode') {
            git branch: 'Sprint1_develop', url: 'https://github.com/kavyaanantha/game-of-life.git'
        }
        stage('Build the code') {

            sh 'mvn clean package'

        }
        stage('Test results') {
            junit '**/surefire-reports/*.xml'
        }

    }