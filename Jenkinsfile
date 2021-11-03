pipeline {
    agent any

    stages {
        stage('java1') {
            steps {
                echo 'Executing first java code'
                bat 'javac One.java'
                bat 'java One'
            }
            
        }
        stage('timeout') {
            steps {
                echo '30 seconds timeout'
                timeout(time: 30, unit: 'SECONDS') {
                 // some block
                  }
                }
            
        }
        stage('java2') {
            steps {
                echo 'Executing Second java code'
                bat 'javac Two.java'
                bat 'java Two'
            }
            
        }
        
        
        
    }
}
