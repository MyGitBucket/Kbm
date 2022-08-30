pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'Jdk'
    }
    stages{
     
        stage('Read pom file'){
            steps {
                echo 'Reading pom.xml file from workspace'
                readFile 'pom.xml'
            }
        }
        stage('Build'){
            steps {
                echo 'Building code'
                sh "mvn clean package"
            }
        }
    }
}
