pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                sh 'mvn clean install'
            }
        }
        stage("Deploy") {
            steps {
                sh 'git remote add heroku https://git.heroku.com/ancient-journey-88701.git'
                sh 'git push heroku'
            }
        }
    }
}