pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout your code from Git repository
                echo 'hello'
            }
        }

        stage('Build and Deploy') {
            steps {
                // Build the Maven project
                bat 'mvn clean package'

                // Copy the WAR file to Tomcat's webapps directory
                bat 'copy C:\\Users\\BISMILLAH\\Desktop\\Devops\\demoP\\target\\HelloWorldProject-*.war "C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0_Tomcat9_temp\\webapps\\ROOT.war"'
            }
        }
    }
}
