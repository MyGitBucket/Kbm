pipeline {
    agent any

    stages {
        stage('Git CheckOut') {
            steps {
                echo 'Checking out code from git repository.'
                git 'https://github.com/MyGitBucket/Kbm.git'
            }
        }
    }
}
