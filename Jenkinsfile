pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                script {
                    // Change directory to where App.java is located
                    dir('src/main/java/com/example') {
                        // Compile the Java program
                        sh 'javac App.java'
                    }
                }
            }
        }
        stage('Run') {
            steps {
                script {
                    // Run the compiled Java program
                    dir('src/main/java/com/example') {
                        sh 'java App'
                    }
                }
            }
        }
    }
}