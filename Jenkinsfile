pipeline {
    agent any

    stages {
        stage('fetch'){
            steps{
                git branch: 'main', url: 'https://github.com/Chetan12-rgb/PHPtestTushar.git'
            }
        }
        stage('check'){
            steps{
                sh 'ls'
            }
        }
        stage('conatiner'){
            steps{
                sh 'docker build -t myphp .'
                sh 'docker run --name my_php -d -p 80:80 myphp '
                
            }
        }
    }
}