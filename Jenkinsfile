pipeline {
    agent any

    stages {
        stage('Github') {
            steps {
                git 'https://github.com/prajwalrs123/Jenkins-java.git'
            }
        }
        stage('Accounts') {
            steps {
                bat '''javac HelloWorld.java
                       java HelloWorld.java'''
            } 
        }
        stage('github') {
            steps {
                git 'https://github.com/prajwalrs123/mavenproject.git'
            }
        }
        stage('maven') {
            steps {
                bat'''mvn test'''
            }
        }
    }
}
