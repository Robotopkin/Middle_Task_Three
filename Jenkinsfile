pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps('Prepare') {
                echo 'Начало пайплайна'
            }
        }
        stage('Parallel') {
            parallel{
                stage('Parallel1') {
                    steps('Parallel1') {
                        echo 'Parallel work 1'
                    }
                }
                stage('Parallel2') {
                    steps('Parallel2') {
                        echo 'Parallel work 2'
                    }
                }
            }
        }
    }
    post('End') { 
        always { 
            echo 'End'
        }
    }
}