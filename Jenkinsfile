pipeline {
    agent any

    stages {
        stage('Git CheckOut') {
            steps {
                echo 'Checking out code from git repository.'
                echo 'Check the workspace'
                echo 'Checked out?'
                git 'https://github.com/MyGitBucket/Kbm.git'
            }
        }
    }
}
