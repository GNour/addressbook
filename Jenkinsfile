pipeline {
    agent any
    
    stages {
        stage ("clone the project") {
            steps {
                git "https://github.com/GNour/addressbook"
            }
            
        }
        
        stage ("compile") {
            steps {
                sh "mvn compile"
            }
        }
        
        stage ("tests") {
            steps {
                sh "mvn test"
            }
        }
        
        stage ("package") {
            steps {
                sh "mvn package"
            }
        }
    }
}
