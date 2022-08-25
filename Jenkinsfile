pipeline {
    agent any
    tools {
        maven 'MAVEN'
        jdk 'JDK'
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }
        stage('Git CheckOut') {
            steps {
                echo 'Checking out code from git repository.'
                git 'https://github.com/MyGitBucket/Kbm.git'
            }
        }
        stage('Read pom file'){
            steps {
                echo 'Reading pom.xml file from workspace'
                readFile 'pom.xml'
            }
        }
        stage('Build'){
            steps {
                echo 'Building code'
                sh "mvn clean install"
            }
        }
    }
}
