pipeline {
    agent any

    stages {
        stage('Test'){
            steps {
                sh 'echo "Test"'
            }
        }
        stage('Deploy'){
            steps {
                sh 'rsync -az www.crossing-aachen.de git_deploy@motorbar.de:/var/www/www.crossing-aachen.de/htdocs'
            }
        }
    }
}
