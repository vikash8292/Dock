pipeline {
    agent any
    tools{
    maven 'MAVEN_HOME'
    }
 
    stages {
        stage('Build') {
            steps {
                echo 'Building the Maven project...'
                sh 'mvn clean package'
            }
        }
        stage('Create Docker Image') {
            steps {
                echo 'Building Docker image...'
                sh 'docker build -t  vikashkumar08/img1 .'
            }
        }
    }
}
