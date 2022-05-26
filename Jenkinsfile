    node('JDK8') {
        stage('SourceCode') {
            git branch: 'Sprint1_develop', url: 'https://github.com/kavyaanantha/game-of-life.git'
        }
        stage('unit test') {
            junit '**/surefire-reports/*.xml'
        }
        stage('Build the code') {

            sh 'mvn clean package'

        }

    }