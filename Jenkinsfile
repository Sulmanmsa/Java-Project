pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout your code from Git repository
                git branch: 'master', url: https://github.com/Sulmanmsa/Java-Project.git
            }
        }

        stage('Build and Deploy') {
            steps {
                // Build the Maven project
                bat 'mvn clean package'

                // Copy the WAR file to Tomcat's webapps directory
                bat 'copy target/HelloWorldProject-1.0-SNAPSHOT.war C:\\path\\to\\tomcat\\webapps\\ROOT.war'
            }
        }
    }
}
