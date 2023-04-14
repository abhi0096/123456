pipeline {
    agent any
    stages {

        stage('Clone') {
            steps {
              git branch: 'main', url: 'https://github.com/abhi0096/python-test.git'
            }
        }

        stage('Run Python Script') {
            steps {
                script{
                    sh'''
                        python3 script.py
                      '''
                }
            }
        }
    }
}
